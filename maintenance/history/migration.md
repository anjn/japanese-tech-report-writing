## 導入文・例文の照合と整理方針

以下は構成案と合わせて合意済みの整理方針。再構築に反映した。

| 原文の箇所 | 再構築時の扱い | 対応する合意 |
|---|---|---|
| frontmatterの対象・説明、冒頭の二層構造と優先順位 | 対象を日本語の技術文書全体へ広げ、執筆とレビューの使い分けを記す。出典とライセンス表記は保持する | 対象範囲・役割分離の合意、C01、C02 |
| 「伝えたい主張に関する説明は、省略すると…」 | 単一の主張に限定せず、利用目的に必要な説明を残す原則にする | B01、L02、L04 |
| 「読者は、読む速度が遅く…」、記憶と注意を有限とする説明 | 読む速度を一律に決めつけず、時間・注意・記憶の限界を良い文章の定義へ統合する | 合意済みの定義 |
| 重複点検の導入、冗長の排除の導入 | 一回だけ書くという絶対条件を外し、役割のない反復の点検へ統合する | L01、Q01〜Q03 |
| 「書く／書かない」の区分、誠実さと未実施項目の関係 | 目的と適用範囲で情報量を判断する説明へ統合する | L02、B04、B05、Z02 |
| パラグラフライティングの導入 | 段落を話題と論理のまとまりとして扱う。すべての段落を論証に限定しない | N01 |
| 「文章の論理にツッコミどころを残さない」 | 判断に必要な論理の不足を点検する。想定できる反論を無制限に先回りしない | E01、R01、K01〜K04 |
| 演出は全面禁止でなく節度とする導入 | 理解に寄与するかで点検し、表現形式だけで禁止しない | V05、E04 |
| LLM表現の導入、「本書の術語…」、末尾の良い例・悪い例 | 特定の書籍への依存を除く。例は残すが、「本章では…」が禁止例と良い例の両方にある不整合をA01の条件で整理する | A01、A02、S01〜S05 |
| 翻訳調の比喩の導入、三つの生成経路の説明 | 生成原因を証明済みの分類として断定せず、点検対象の傾向として記す | Z01、A03、X05 |
| carry/open/liveなどの対比例、モデルやデータの擬人化の例、話し言葉の例 | 意味が保たれる文脈を添えて残す。「線形」を加える例は置き換える。元の語だけから観測結果や機構を作らない | A03、A04、V04、X05 |
| 見出しの導入 | 対象・問い・結果・操作を探せる見出しにする | C03、T05 |

レビュー用の具体例は一律に削らない。規範の適用判断に役立つものを残し、条件が必要な例には条件を添える。統合した規範も、原文のどの項目を引き継いだか追跡できるようにする。

## 再構築の構成案

状態：構成は合意済み。本文を再構築済み。

### SKILL.md：毎回読む短い入口

1. 利用目的と対象文書
2. 良い文章の定義（正確さ、必要情報、読み手の負荷）
3. 共通原則（目的・読者、根拠と確度、必要な条件、情報の順序）
4. 執筆とレビューの使い分け、必要な参照資料へのリンク

執筆依頼では文書種別に応じたガイドを読む。レビューの詳細規範は初稿を書く前に一括で読ませず、初稿後の見直しやレビュー依頼で読む。レビューだけの依頼では、対象文書に必要な範囲を点検する。

### references/writing.md：文書の役割ごとの執筆ガイド

- レポート：目的、結論、結果、根拠、限界。
- 手順書：前提、操作、成功判定、失敗時の対応。
- 技術解説：概念の導入、前提、仕組み、例。
- 仕様書・リファレンス：対象、項目、条件、参照のしやすさ。
- 設計・判断の記録：選択肢、判断理由、当時の条件、後日の追跡。

固定テンプレートとして全節を必須にしない。執筆に必要な構成判断を短く示し、語句ごとの禁止事項は置かない。

### references/review.md：レビュー手順と詳細規範

1. 内容と構成：目的との対応、根拠・確度、情報の過不足、条件と再現性。
2. 読み手の負荷：順序、段落、参照、図表、必要な再掲。
3. 日本語の表現：空疎な表現、直訳・比喩、用語、接続、語調、演出。
4. 修正後の確認：意味・条件・数値・不確実性の保持、参照先の整合。

各規範には適用条件と役立つ例を残す。指摘や修正は、どの読者負担や誤読を減らすかに基づける。読みやすい箇所まで好みで書き換えない。全チェック項目をレビュー結果へ列挙する必要はない。

### REVIEW.md：検討履歴と移行の対応

実行時に毎回読む資料にはせず、採否と移行先を確認する記録として保持する。再構築時に各IDの移行先を付け、統合による削除と不採用を区別する。

## 次の作業

本文を再構築済み。実際の執筆・レビューで得られた結果に基づいて規範と配置を調整する。


## 再構築後の移行先

各項目の実行用規範をレビュー資料へ統合した。判断理由と比較用の原文はこの記録に保持する。執筆時の原則はSKILL.md、文書別の構成判断はreferences/writing.mdへ要約している。C02の不採用判断はこの記録に残し、実行用資料には情報を演出のために伏せない方針だけを記す。新しい文書種別のガイドは合意した利用目的に基づく追加である。

| ID | 項目 | 詳細の移行先 |
|---|---|---|
| [R01](topics/evidence.md#r01) | 推量を断定に変えない | references/review.md の「根拠と不確実性」 |
| [R02](topics/evidence.md#r02) | 因果の説明 | references/review.md の「根拠と不確実性」 |
| [R03](topics/evidence.md#r03) | 断定を強める推敲 | references/review.md の「根拠と不確実性」 |
| [R04](topics/terminology.md#r04) | 定義を置く位置 | references/review.md の「用語と対象の明確さ」 |
| [R05](topics/evidence.md#r05) | 例の現実性を支える根拠 | references/review.md の「根拠と不確実性」 |
| [B01](topics/purpose.md#b01) | 書き始める前の確認 | references/review.md の「目的と情報の過不足」 |
| [B02](topics/procedures.md#b02) | 手順から推測できる説明 | references/review.md の「手順と実行条件」 |
| [B03](topics/purpose.md#b03) | 失敗した試行の経緯 | references/review.md の「目的と情報の過不足」 |
| [B04](topics/purpose.md#b04) | 実施していない項目 | references/review.md の「目的と情報の過不足」 |
| [B05](topics/evidence.md#b05) | 確認していない事実 | references/review.md の「根拠と不確実性」 |
| [K01](topics/logic.md#k01) | 異なる対象の区別 | references/review.md の「概念と論理の整合」 |
| [K02](topics/logic.md#k02) | 複数の要因の区別 | references/review.md の「概念と論理の整合」 |
| [K03](topics/logic.md#k03) | 概念の一貫性 | references/review.md の「概念と論理の整合」 |
| [K04](topics/evidence.md#k04) | 主張と例の対応 | references/review.md の「根拠と不確実性」 |
| [K05](topics/repetition.md#k05) | 参照先の確認 | references/review.md の「重複と参照の負担」 |
| [T01](topics/evidence.md#t01) | 保証や解決の断定 | references/review.md の「根拠と不確実性」 |
| [T02](topics/logic.md#t02) | 譲歩で認める内容 | references/review.md の「概念と論理の整合」 |
| [T03](topics/logic.md#t03) | 否定の対象と根拠 | references/review.md の「概念と論理の整合」 |
| [T04](topics/terminology.md#t04) | 術語に見える一般表現 | references/review.md の「用語と対象の明確さ」 |
| [T05](topics/structure.md#t05) | 見出しの内容と形式 | references/review.md の「構成と見出し」 |
| [L01](topics/repetition.md#l01) | 主張の反復 | references/review.md の「重複と参照の負担」 |
| [L02](topics/purpose.md#l02) | 情報を残す基準 | references/review.md の「目的と情報の過不足」 |
| [L03](topics/procedures.md#l03) | 成功判定の参照 | references/review.md の「手順と実行条件」 |
| [L04](topics/procedures.md#l04) | 説明の短縮 | references/review.md の「手順と実行条件」 |
| [L05](topics/repetition.md#l05) | 文字数と冗長さ | references/review.md の「重複と参照の負担」 |
| [C01](topics/structure.md#c01) | 結論と反論の順序 | references/review.md の「構成と見出し」 |
| [C02](topics/structure.md#c02) | 情報の先出し | references/review.md の「構成と見出し」 |
| [C03](topics/structure.md#c03) | 結論を示す見出し | references/review.md の「構成と見出し」 |
| [C04](topics/structure.md#c04) | 本文の固定順序 | references/review.md の「構成と見出し」 |
| [M01](topics/paragraphs.md#m01) | 未知の概念を説明する順序 | references/review.md の「段落と説明の順序」 |
| [M02](topics/terminology.md#m02) | 抽象語の指す対象 | references/review.md の「用語と対象の明確さ」 |
| [M03](topics/examples.md#m03) | 例を追加する理由 | references/review.md の「例と媒体間の対応」 |
| [M04](topics/paragraphs.md#m04) | 並列の事実を一文にまとめること | references/review.md の「段落と説明の順序」 |
| [M05](topics/terminology.md#m05) | 説明を名称に置き換えること | references/review.md の「用語と対象の明確さ」 |
| [D01](topics/paragraphs.md#d01) | 対比する定義の文型 | references/review.md の「段落と説明の順序」 |
| [D02](topics/logic.md#d02) | 限定の後に必ず論を進めること | references/review.md の「概念と論理の整合」 |
| [D03](topics/logic.md#d03) | 上位概念でまとめること | references/review.md の「概念と論理の整合」 |
| [D04](topics/repetition.md#d04) | 前方参照の位置 | references/review.md の「重複と参照の負担」 |
| [D05](topics/terminology.md#d05) | 人物名の表記 | references/review.md の「用語と対象の明確さ」 |
| [N01](topics/paragraphs.md#n01) | 段落の話題と冒頭 | references/review.md の「段落と説明の順序」 |
| [N02](topics/paragraphs.md#n02) | 隣接する節の統合 | references/review.md の「段落と説明の順序」 |
| [N03](topics/repetition.md#n03) | 説明直後の要約 | references/review.md の「重複と参照の負担」 |
| [N04](topics/paragraphs.md#n04) | 読み進める間に保持する情報 | references/review.md の「段落と説明の順序」 |
| [N05](topics/examples.md#n05) | 例に不要な詳細 | references/review.md の「例と媒体間の対応」 |
| [Q01](topics/repetition.md#q01) | 数値の再掲の削除 | references/review.md の「重複と参照の負担」 |
| [Q02](topics/repetition.md#q02) | 説明と確認事項の重複 | references/review.md の「重複と参照の負担」 |
| [Q03](topics/repetition.md#q03) | 同じ主張と必要な反復の区別 | references/review.md の「重複と参照の負担」 |
| [Q04](topics/repetition.md#q04) | 補足を置く位置 | references/review.md の「重複と参照の負担」 |
| [Q05](topics/purpose.md#q05) | 削除してよい段落の判断 | references/review.md の「目的と情報の過不足」 |
| [P01](topics/procedures.md#p01) | 各手順の必須情報 | references/review.md の「手順と実行条件」 |
| [P02](topics/procedures.md#p02) | 前提と注意の位置 | references/review.md の「手順と実行条件」 |
| [P03](topics/procedures.md#p03) | ファイル配置のツリー | references/review.md の「手順と実行条件」 |
| [P04](topics/procedures.md#p04) | 置換箇所と実行可能性 | references/review.md の「手順と実行条件」 |
| [P05](topics/figures.md#p05) | 同じ内容を複数の媒体で示すこと | references/review.md の「図表とコードの提示」 |
| [F01](topics/structure.md#f01) | 概要に含める数値 | references/review.md の「構成と見出し」 |
| [F02](topics/structure.md#f02) | 題名と副題 | references/review.md の「構成と見出し」 |
| [F03](topics/figures.md#f03) | 表・グラフの選択 | references/review.md の「図表とコードの提示」 |
| [F04](topics/figures.md#f04) | 図表に添える条件 | references/review.md の「図表とコードの提示」 |
| [F05](topics/figures.md#f05) | スクリプト全文の配置 | references/review.md の「図表とコードの提示」 |
| [X01](topics/examples.md#x01) | 例についての補足を置く位置 | references/review.md の「例と媒体間の対応」 |
| [X02](topics/examples.md#x02) | 説明用の例であることの明示 | references/review.md の「例と媒体間の対応」 |
| [X03](topics/examples.md#x03) | 図・表・コードの対応 | references/review.md の「例と媒体間の対応」 |
| [X04](topics/terminology.md#x04) | まだ導入していない対象への言及 | references/review.md の「用語と対象の明確さ」 |
| [X05](topics/expressions.md#x05) | 不自然な比喩の点検方法 | references/review.md の「空疎な表現と不自然な比喩」 |
| [A01](topics/expressions.md#a01) | 予告と総括 | references/review.md の「空疎な表現と不自然な比喩」 |
| [A02](topics/expressions.md#a02) | 空虚な形容・動詞 | references/review.md の「空疎な表現と不自然な比喩」 |
| [A03](topics/expressions.md#a03) | 無生物主語と擬人化 | references/review.md の「空疎な表現と不自然な比喩」 |
| [A04](topics/expressions.md#a04) | 比喩を具体化する際の意味の保持 | references/review.md の「空疎な表現と不自然な比喩」 |
| [A05](topics/style.md#a05) | 形容詞＋「です」 | references/review.md の「文体・語り・強調」 |
| [W01](topics/style.md#w01) | 文書の種類と文体 | references/review.md の「文体・語り・強調」 |
| [W02](topics/terminology.md#w02) | 日本語訳と原語 | references/review.md の「用語と対象の明確さ」 |
| [W03](topics/terminology.md#w03) | 固有名と識別子の省略 | references/review.md の「用語と対象の明確さ」 |
| [W04](topics/paragraphs.md#w04) | 接続表現の必須化 | references/review.md の「段落と説明の順序」 |
| [W05](topics/procedures.md#w05) | 操作の禁止を婉曲にすること | references/review.md の「手順と実行条件」 |
| [E01](topics/logic.md#e01) | 誤解の先回り | references/review.md の「概念と論理の整合」 |
| [E02](topics/style.md#e02) | 読者との架空の問答 | references/review.md の「文体・語り・強調」 |
| [E03](topics/style.md#e03) | 行為者を主語にした説明 | references/review.md の「文体・語り・強調」 |
| [E04](topics/style.md#e04) | 太字の回数制限 | references/review.md の「文体・語り・強調」 |
| [E05](topics/procedures.md#e05) | 事故や危険の列挙 | references/review.md の「手順と実行条件」 |
| [V01](topics/style.md#v01) | 読者への呼びかけ | references/review.md の「文体・語り・強調」 |
| [V02](topics/style.md#v02) | 架空の人物設定 | references/review.md の「文体・語り・強調」 |
| [V03](topics/terminology.md#v03) | 用語の具体性と慣用 | references/review.md の「用語と対象の明確さ」 |
| [V04](topics/expressions.md#v04) | 話し言葉による曖昧な評価 | references/review.md の「空疎な表現と不自然な比喩」 |
| [V05](topics/style.md#v05) | 緊張や山場を作る演出 | references/review.md の「文体・語り・強調」 |
| [S01](topics/expressions.md#s01) | 姿勢だけを宣言する言葉 | references/review.md の「空疎な表現と不自然な比喩」 |
| [S02](topics/paragraphs.md#s02) | 接続の型とリズム | references/review.md の「段落と説明の順序」 |
| [S03](topics/evidence.md#s03) | 弱い緩和と称賛 | references/review.md の「根拠と不確実性」 |
| [S04](topics/expressions.md#s04) | 接続や評価だけの文 | references/review.md の「空疎な表現と不自然な比喩」 |
| [S05](topics/expressions.md#s05) | 発想のメタな紹介と著者の弁明 | references/review.md の「空疎な表現と不自然な比喩」 |
| [Z01](topics/expressions.md#z01) | 案内・強調・比喩 | references/review.md の「空疎な表現と不自然な比喩」 |
| [Z02](topics/figures.md#z02) | 残す根拠・注意・手順と図表の役割 | references/review.md の「図表とコードの提示」 |
| [Z03](topics/procedures.md#z03) | 手順の番号と準備の区別 | references/review.md の「手順と実行条件」 |
| [Z04](topics/style.md#z04) | 例文の文体と本文の統一 | references/review.md の「文体・語り・強調」 |
| [Z05](topics/terminology.md#z05) | 単位・略語と識別子 | references/review.md の「用語と対象の明確さ」 |

## 再構築後の確認

- 94項目すべてについてレビュー資料内の移行先を確認した。原文の引用はこの記録に保持し、実行用の資料からは旧規範の引用を除いた。
- スキル形式の検証を実施した。
- 次の短い例で、規範同士の整合を机上確認した。独立したモデルによる実行評価ではない。

| 場面 | 確認した扱い |
|---|---|
| 数値のない設計調査の初稿 | 目的・結論・条件を示し、概要の形式のために数値を加えない。F01と執筆ガイドが一致する。 |
| 手順の期待値が概要にも記載されている | 操作の近くに期待値を残す。L01、L03、Q01、Q02が矛盾しない。 |
| 「有効かもしれない」を強い表現へ推敲する | 根拠を確認せず「必須」と断定しない。R01、R03、S03と具体例が一致する。 |
| 「サーバーが応答を返します」をレビューする | 無生物主語を理由に書き換えない。A03と執筆の自由を保つ原則が一致する。 |

## レビュー資料の簡潔化

利用者の提案に基づき、references/review.mdから目的・採否・判断理由・適用段階・検討IDを除いた。内容を削るだけでなく、理由欄に含まれていた適用条件を規範へ移し、同じ指示をテーマ別に統合した。判断記録は本ファイルに維持し、94項目の移行先表を現在の見出しへ更新した。表現の具体例は維持した。
