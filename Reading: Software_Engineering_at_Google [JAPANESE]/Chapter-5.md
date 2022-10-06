# チームリーダー入門

Google には 2 種類の異なるリーダーシップ役職がある。

- エンジニアリングマネージャー：人員のリーダー
- テックリード：技術的取り組みの主導

## マネージャーとテックリード

各役職に求められるスキルは甚だしく異なる。

- エンジニアリングマネージャー (EM)

  - Google は以下を資質とする
    - 経験を積んだマネージャでかつてソフトウェアエンジニアだった者
    - ソフトウェアエンジニアを訓練してマネージャとすること
  - より高いレベルでは以下を求める
    - チームが担当する製品がビジネス要件を満たすことを保証する
    - テックリードを含むチーム内全ての人員の成績、生産性、満足度に責任を持つ
  - ビジネス要件と個々のチームメンバーの要求は必ずしも相容れない
    - これは、マネージャを難しい立場に置く

- テックリード (TL)

  - チームのマネージャの部下である場合も多い
  - 製品の技術的側面を担当する、具体的には以下
    - 技術的な決定と選択
    - アーキテクト
    - 優先度
    - 開発速度
    - プロジェクト管理一般等
  - エンジニアリングマネージャと二人三脚で仕事をする
    - チームに十分な人員がいることを保証する
    - エンジニアが自分たちのスキルセット・レベルに沿ったタスクに取りかかれるように保証する
  - 大半の TL は IC でもある。このため以下の選択を強いられる。
    - 自身で何かを手っ取り早くやってしまう
    - チームメンバーに任せて、時間をかけて行ってもらう
    - ほとんどの場合、後者が正しい判断である

- テックリードマネージャー (TLM)

  - 小規模チームには TLM がいる場合が多い
    - TLM は TL と EM の両方に対処できる人物である
    - 通常は、最近まで IC だった者がこの役職を務める
  - TLM が学ばなければならないことが多い
    - 通常は、より熟練した TLM からの高度なメンタリングと支援を要する
  - Google では、TL 1 人・EM 1 人とチームメンバーの構成が通例である
    - 2 人のスペシャリストが専任で各々の役目を攻略している

## サーバントリーダーシップ

- 従業員の積極的な「管理」は基本的に、悲惨な結果に終わる
- Google のエンジニアリングディレクターいわく「何よりも、管理しようとする衝動に抵抗せよ」
- マイクロマネジメント、成績の悪いもの無視、押しに弱い人間の採用は、マネージャのかかるある種の病である
- この病にはサーバントリーダーシップが有効である
  - サーバントリーダーは、謙虚・尊敬・信頼からなる雰囲気の醸成に励むべきである
  - 執事が家令や一家の健康と充足に気を配ることと似た位置づけである
  - サーバントリーダーの責務は、チームの技術的健全性ならびに社会的健全性の管理
    - 複雑な形式的手続き上の障害で、チームメンバー自身が取り除けない課題の除去
    - チーム内の合意形成の手伝い
    - 必要時にはチームにアドバイスを与える
    - 自ら手を動かすことを厭わない

## エンジニアリングマネージャー

- 伝統的なマネージャは物事をやり遂げる方法を気にする
- 優れたマネージャはどんな物事がやり遂げられるのかを気にする
  - やり遂げる方法はチームに任せる

## アンチパターン

- 押しに弱い者を採用する

  - 自分の権限に意義を唱えられたり、職を脅かされたりしない手段である
    - これによりチームリーダーや意思決定者としての自分の立場は確立される
    - 反面、これは自分の仕事が増えることに繋がり、その者は休暇がとれなくなる
    - その者がチームを離れた瞬間、生産性が急停止する
  - マネージャーは、自身より賢く、交代できる者を採用するよう務めるべきである
    - その者は、定期的に盾突き、マネージャを唸らせることになる
    - あるいは、チームを率いたいと熱望する者もいる
    - これらは学びと成長のチャンスであり、いずれも歓迎すべきである
      - 前者は、マネージャ自身が新しい観点を調べる機会に繋がる
      - 後者は、追加のチームを率いることに繋がる
    - この環境に身を置くと、専門知識を広げるのが容易になる

- 成績の悪い者を無視する

  - 人間を扱う際に最も困難な要素は、期待に応えていない者の扱いである
  - 最も難しい事例は、どんなに長時間もしくは勤勉に働こうが、職務遂行能力が全く無い場合である
  - 成績の悪い者を効果的に指導するにはどうすればよいか
    - 最適な類推は、その者が自律的にあるき出し、ゆっくり走り、チームの他のものに並走する過程を手伝うことである
    - この指導は、一時的にはマイクロマネジメントを要することがほぼ常である
    - ただし、その中でも謙虚、尊敬、信頼は必要である、特に尊敬は重要である
    - タスクは 2 ヶ月程度の期限で達成出来る具体的なゴールを設定すると良い
    - 小さな成功の機会が多くあるように、ゴールは小さく、インクリメンタルで、計測可能な物にすべきである
    - 毎週そのチームメンバーと会って進捗確認し、明示的な期待要件を必ず設定すべきである
      - 本当に職務遂行能力がない者は、このプロセスの過程で明らかになる。結果、
        - 腕を上げ、期待に添えるようになる
        - または、辞めることを決断する
    - いずれにせよ、マネージャは、成績の悪いものと直接仕事をし、重要かつ必要な変化の触媒となるべきである

- 人間的問題を無視する

  - マネージャは、チームのために 2 つの主要な関心領域を持つべきである
    - 社会的な関心
    - 技術的な関心
  - エンジニアから昇進したマネージャは、技術的な関心に力を入れがちである
  - マネージャがチームの人間的要素を無視するのは、自殺行為に他ならない
    - 例：妻子持ちでリモートワーク主体の優秀なエンジニアに、チームの都合で全日出社を要求する
      - 人間性に共感し、お互いに譲歩出来るラインを交渉すべきである

- 全員の友人になる

  - マネージャは、以前メンバーだったチームのマネージャになることが多い
    - 多くのリーダーは自分のチームとメンバー達との間に育んだ友情を失いたくない
    - チームのリーダーになってから、メンバーとの友情を維持すべく特に熱心に務める
      - これは、大惨事ならびにたくさんの友情の崩壊がほぼ必至である
      - 友情を、人当たりよくチームを率いることと混同してはならない
      - キャリアに対して責任を持つ者と持たれる者の間には一線が必要である
  - 自分のチームと親しい友人関係にならずとも、チームを率いて合意形成は可能である
    - 同様に、既存の友情を投げ捨てなくても強靭なリーダーにはなれる

- 採用基準で妥協する

  - Steve Jobs 曰く「A 級の人々は A 級の人々を採用する。B 級の人々は C 級の人々を採用する」
  - チームがエンジニアを 5 人採用する目標があり、大量の応募から最優秀者 5 人を選ぶのは、二流チームを作る最速の方法である
    - 採用基準は絶対である、その 5 名がその基準を満たさない場合は目標を妥協すべきである
    - 適切な人物を見つけ出すコストは、絶対に雇うべきではなかった従業員に対処するコストからすれば安い
    - コストの例
      - チームの生産性消失とストレス
      - その従業員が頭角を表さない場合に解雇するまで管理する時間
      - 解雇の書類事務とストレス etc
  - 素晴らしいチームを作る材料なくしては、破滅が待つのみである

- 自分のチームを子供のように扱う

  - マイクロマネジメントや、メンバーの能力を軽んじて仕事を担当する機会を与えなかったりすること
  - 信頼出来るメンバーを採用し、その者に期待していることを示すだけで良い

## 建設的パターン

- エゴを捨てよ

  - 肥大した個人的エゴは扱いにくく、チームリーダーが持つエゴは特に注意が必要である
  - リーダーは、集団的なチームとしてのエゴと主体性を育成し強化するように務めるべきだ
  - 失敗したときに謝れるリーダーには、人は並外れて大きな敬意を払う

- 禅の労使となれ

  - 優れたエンジニアは、的確な懐疑と皮肉の感覚を持ち合わせる
  - 反面、チームを率いる際には大きな負債となりうる
  - 自分の印象を伝え、平成を保つことが、より多くのものを率いるようになるにつれて重要となる
    - この結果、チームメンバーは、行動の方法と周囲の事象に対応する方法について、手がかりを求めてリーダーを頼る

- 触媒となれ

  - 化け学における触媒とは、化学反応を促進させるがその反応の中でそれ自体は消耗しない
  - 触媒が作用する形式の一つは、反応物質をかたわらへ運ぶことであり、マネージャの動きと通ずる
  - チームリーダーが行う最も一般的なことは、合意形成である

- 障害を取り除け

  - チームは障害に突き当たって停滞することがある
  - リーダーは、チームが再び動けるように助けに入るべきである
  - リーダーは、メンバーが持たない対処手段を持っている

- 先生かつメンターになれ

  - 優れたメンターは、メンティーの学習時間とメンティーが製品に貢献する時間との間のトレードオフのバランスを取らなければならない
  - 自分が 20 分以内に片付けてしまえるとわかっていても、自分よりジュニアなチームメンバーが 3 時間費やすことを見守ることは妥当である

- 明確なゴールを設定せよ

  - リーダーは、チームをある方向へ急速に向かわせようとするなら、その方向を明確にしなければならない
  - 加えて、明確なゴールを持つなら、明確な優先度を設定する必要がある
  - トレードオフが必要になった時は、どのように処理するか、決めるのを手伝わなければならない
  - ミッションステートメントは、チームを同じ方向に進ませるための最も簡単な方法だ

- 正直であれ

  - 情報共有出来ない内容をメンバーからの質問された場合は「知らない」ではなく「知っているが答えることは出来ない」で良い
  - マネージャの職にある多くの人々は、なにかに対する応えを知らないと、自分たちが劣っていたり事情に疎かったりすると証明されると感じる
    - 本当に知らないことを聞かれた場合は、知らないと応えて良い
  - マネジメント本は、部下に厳しいフィードバックを与える時に「褒め言葉のサンドイッチ」を使えと示すがそれは回避すべきである

    > 例：君はチームの信頼出来るメンバーで、エンジニアの中で賢い部類だ。
    > その上でなんだけど、君のコードはややこしくてチームの誰にとってもほとんど理解不能なんだ。
    > でも君はすごく見込みがあるし、めちゃくちゃイケてる T シャツのコレクションも持っているね。

    - 多くの人は、良い部分だけを受け止め、決定的な重要なメッセージを捉えそこねる
    - しっかり尊敬の念を持ちつつ、思いやりと共感をもって、ロジカルに批判を伝えると良い

      > 我々は君が認識出来ていないと思っているため、あえて告げるが、君のチームとの関わり方は不和を生み反感を買う類のものだ。
      > もし君がチームの役に立ちたいなら、コミュニケーションのスキルを磨かないといけないし、君がスキルを磨く手助けに我々はコミットするよ。

- 満足度を追跡調査せよ

  - リーダーの立場からチームの生産性を長期で上げるには、チームの満足度を測ることに時間を投資すると良い
  - 満足度を追跡調査するための、簡単で優れた方法は、毎回の 1:1 面談の最後にチームメンバーに「何が必要かな」と尋ねることだ
  - この単純な質問は、話を締めくくり、生産的かつ充足した状態であるために必要なものを、各メンバーが入手出来ていることを確認する良い方法である

## ヒント

Google で推奨しているリーダーシップ職位についている者の行動例。

- 委譲する、しかし手は動かす
- 自分の代わりを探す
- 波風を立てるべきときを心得る
- チームを混沌から守る
- チームの上空援護をする
- チームがうまくやっているときはそれをチームに伝える
- もとに戻すものが簡単なものに「イエス」というのは容易い

## 「内発的動機付け」と「外発的動機付け」

- 動機付けには 2 　つのパターンが存在する
  - 「外発的動機付け」：年収等
  - 「内発的動機付け」：自主性、熟達、目的
- 人の満足度を高め生産性を上げることが出来るのは、後者である
- 自主性とは、メンバーを信頼し、物事を任せることを意味する
  - これにより、製品はより良い形を目指せる
  - また、製品が成功するのを見届けることへの関心にも繋がる
- 熟達とは、既存のスキルを伸ばし、新たなスキルを得る機会を与えることを意味する
  - 機会を与えることは、時間とともに人を成長させる
  - これは、チームの強化にも繋がる
  - Google は、エンジニアを背鋭敏で能率的で即戦力となる状態に維持しておくべく、新しいことを学び、技能に熟達するために十分な機会をエンジニアに与えている
- 自主性も熟達も、目的なくしては成立しない
  - チームが努力する理由を探し、その理由をチームに明確にすることは必要だ
  - チームが仕事の目的を認識出来れば、その生産性は凄まじく上昇する

## まとめ

- 伝統的な意味での「管理」は行うな。リーダーシップ、影響力、チームに使えることに集中せよ。
- 可能な場合は委譲せよ。DIY (Do It Yourself：自前作業) は行うな。
- チームの着眼点、方向、速度に特に注意を払え。