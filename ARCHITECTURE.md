# Architecture

My golang code is inspired by the domain-driven design born from JavaScript.

- My friend writes similar document for JavaScript. Please refer to [r-sylph/web](https://github.com/r-sylph/web/blob/master/.github/ARCHITECTURE.md) if you want.

## Rules

- Single direction data-flow

  - All layers should be implemented with the knowledge only they have.
  - Only domain layer can provide entities and object to other layers.

- Modulable components

  - Modules should be split into appropriate granularity.
  - Function and module should be keep lightweight.

## Directory Structure

- The structure is a hybrid of DDD and [golang-standards/project-layout](https://github.com/golang-standards/project-layout).

  | Directory               | Description                                                                                                                                                                                          |
  | :---------------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
  | cmd                     | Entrypoint for the app. <br>This directory is based on [golang-standards/project-layout#cmd](https://github.com/golang-standards/project-layout#cmd).                                                |
  | cli                     | Command-line interface such as `cobra` and `urfave/cli`. <br>This code read user-defined parameters such as `listen-address` and `listen-port`.                                                      |
  | internal                | Private application and library code. <br>This directory is based on [golang-standards/project-layout#internal](https://github.com/golang-standards/project-layout#internal)                         |
  | internal/domain         | App-specific domain entities and objects.<br>No use knowledge of other layers, store only pure domain knowledge.                                                                                     |
  | internal/config         | App-specific config loader and validator.<br>This layer inspects persistent configs written by YAML for the most part.                                                                               |
  | internal/framework      | Framework such as `Echo`, `Gin` and `os/exec`.<br>This layer invokes routes and middlewares using Cotroller.                                                                                         |
  | internal/application    | Business and application logics.<br>This layer invokes app-specific usecases using Controller.                                                                                                       |
  | internal/infrastructure | Interface adapters such as `API Client`, `DB Client` and `io/fs`.<br>This layer invokes external repositories and also remodel their data.                                                           |
  | pkg                     | Imported external libraries. They will be invoked from internal layers. <br>This directory is based on [golang-standards/project-layout#pkg](https://github.com/golang-standards/project-layout#pkg) |

## Data-flow Overview

- Go through a request from left layer to right layer.
- Invoke Modules (router, middleware, usecase and repository) from upstream layer.
- Write a test for the public method of each module.

  ```plaintext
  +-------------------------------------------------------------------------------------+
  |                                       domain                                        |
  +-------------------------------------------------------------------------------------+

                 +------------+              +-----------+               +--------------+
          +----< | Router     |       +----< | Usecase A |        +----< | Repository A |
          |      +------------+       |      +----------+         |      +--------------+
          +----< | Middleware |       +----< | Usecase B |        +----< | Repository B |
          |      +------------+       |      +-----------+        |      +--------------+
          |                           |                           |
    +-----+------+              +-----+------+              +-----+------+
    | Controller |              | Controller |              | Controller |
    +-----+------+              +-----+------+              +-----+------+
          |                           |                           |
    +=====+=============+       +=====+=============+       +=====+=============+
    |     Framework     | ----> |    Application    | ----> |  Infrastructure   |
    |     (CLI/API)     |       |     (Usecase)     |       |   (Repository)    |
    +=====+=============+       +=====+=============+       +=====+=============+
          |                           |                           |
  +-------+---------------------------+---------------------------+----------------------+
  |                                        config                                        |
  +--------------------------------------------------------------------------------------+
  ```

## Examples

- [umatare5/telee](https://github.com/umatare5/telee)
- [umatare5/atmos-cli](https://github.com/umatare5/atmos-cli)
- [umatare5/logbook-api](https://github.com/umatare5/logbook-api)
