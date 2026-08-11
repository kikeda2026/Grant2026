# DSM 日英テキスト対照表
# Japanese–English Text Reference for DSM (Digit Symbol Matching)

# 作成日 / Created: 2026-08-11
# 対象ファイル / Source file: DSM_Main.v1.Jul24.html
#
# 原典 / Source:
#   TestMyBrain Digit Symbol Matching (TMB DSM)
#   The Many Brains Project (manybrains.net) — GNU LGPLv3
#   Original task adapted from WAIS-III (Wechsler, 1997)
#
# 本研究での修正内容 / Modifications for this study:
#   - 標準版（90秒・6シンボル）をそのまま使用
#   - 全テキストを日本語化
#   - 練習ページ専用のseed値（990001）を使用。本番用seed値は未定（cognitive.html実装時に確定）
#   - 試行完了後にGASへデータを自動送信（練習ページでの実施を除く）
#   - Standard version (90 seconds, 6 symbols) used as-is
#   - All UI text translated to Japanese
#   - Dedicated practice-page seed (990001); production seed values TBD
#     (to be confirmed when cognitive.html is implemented)
#   - Auto-submit results to GAS on completion (except when run from practice.html)
#
# 参照 / Reference:
#   Chaytor et al. (2021); Hawks et al. (2023); Singh et al. (2021, 2023)
#   Task overview: Task_Overview_TMB_Digit_Symbol_Matching.pdf
#   Dictionary/URL params: TMB_DSMDictionary_v1_Jul24.xlsx
#
# 用語について / Note on terminology:
#   GradCPT_JP_EN_text.mdと同じ方針で，「本番」は研究1トップページの
#   「今日の認知課題」（cognitive.html）経由のデータ収集セッションのみを指す。
#   練習課題ページ（practice.html）で実施する内容（90秒テストを含む）は
#   すべて「練習」であり，参加者向けの文言では「本番」ではなく「テスト」と表現する。
#   Same convention as GradCPT_JP_EN_text.md: "本番" refers only to the daily
#   data-collection session via cognitive.html. Everything on practice.html,
#   including its full 90-second test, is "practice" and is referred to as
#   "テスト" (test), never "本番," in participant-facing text.

---

## 1. タイトル画面 / Title Screen

| 日本語 | English (Original) |
|--------|-------------------|
| 形とシンボルのマッチング | Matching Shapes And Numbers |

---

## 2. 説明画面 / Instruction Screen

| 日本語 | English (Original) |
|--------|-------------------|
| 説明： | Instructions: |
| それぞれの**シンボル**には**数字**が対応しています。 | Each **symbol** has a **number**. |
| 画面上部にシンボルが表示されたら，（タップ版）対応する数字を**画面でタップ**してください（これは1です）。 | When a symbol appears at the top,<br>**touch** its number **on the screen**<br>(here it is 1). |
| 画面上部にシンボルが表示されたら，（キーボード版）対応する数字を**キーボード**で押してください（これは1です）。 | When a symbol appears at the top,<br>press its number on the **keyboard**<br>(here it is 1). |

---

## 3. 練習移行メッセージ / Practice Transition Messages

| # | 日本語 | English (Original) |
|---|--------|-------------------|
| 練習開始前 | いくつかのシンボルで練習しましょう。 | Let's practice a few symbols. |
| 練習完了後 | よくできました！練習が終わりました。続けてテストを行います。 | Excellent!<br>You have completed the practice.<br>Now let's do more. |

**用語について：** 原文の後半（"Now let's do more"）は，本研究では「続けてテストを行います」と訳し，GradCPTと同様に「本番」の語を使わない。
**Note:** The original's latter half ("Now let's do more") is rendered as "続けてテストを行います" (we'll now do the test), avoiding "本番" per the same convention as GradCPT.

---

## 4. テスト説明メッセージ / Test Introduction Message

| 日本語 | English (Original) |
|--------|-------------------|
| 得点は，X秒間にどれだけ正しく回答できたかで決まります。**正確に**，そして**すばやく**答えましょう！ | Your score will be<br>how many correct responses<br>you make in X seconds,<br>so try to be **ACCURATE** and **QUICK**! |

「X秒間」の値は`duration`パラメータ（既定90秒）が動的に挿入される。
"X seconds" is dynamically filled from the `duration` parameter (default 90).

---

## 5. 練習試行のやり直し画面 / Practice Retry Screen

練習トライアルで無反応または誤答だった場合に表示。同じシンボル画像とともに表示される。
Shown when a practice trial times out or is answered incorrectly, alongside the same symbol image.

### (タップ版 / Touch version)

| 日本語 | English (Original) |
|--------|-------------------|
| もう一度：<br>このシンボルが出たら**Nをタップ**してください。 | Remember:<br>**touch the screen** to respond.<br>You should **touch N** |
| タップしてやり直す（ボタン） | Click here to retry |

### (キーボード版 / Keyboard version)

| 日本語 | English (Original) |
|--------|-------------------|
| もう一度：<br>このシンボルが出たら**N**を**キーボード**で押してください。 | Remember:<br>**use the keyboard** to respond.<br>You should **press N** on the **keyboard** |
| スペースキーを押してやり直す（ボタン） | Press the SPACEBAR to retry |

---

## 6. 画面遷移ボタン文言 / Continue / Advance Button Labels

begin・messageタイプのフレーム（各説明画面）で共通して使用。GradCPTと同一の文言規則。
Used across all "begin" and "message" type frames. Same wording convention as GradCPT.

| 画面 | タップ版 | キーボード版 |
|------|---------|------------|
| 冒頭の説明へ進む（begin） | タップして説明を見る | スペースキーを押して説明を見る |
| 通常の「続ける」（message） | タップして続ける | スペースキーを押して続ける |

---

## 7. 練習スキップ画面 / Practice Skip Screen（nopractice=optional時のみ）

**現在未使用：** GradCPTと同様，本研究のURL呼び出しでは`nopractice`を`'optional'`に設定しないため，参加者がこの画面を見ることはない。ラジオボタンの選択肢テキストは未翻訳のまま（英語）。
**Currently unused:** As with GradCPT, this study never sets `nopractice` to `'optional'`, so participants never see this screen. Its radio-button option text remains untranslated (English).

| 日本語 | English (Original / 現状のまま未翻訳) |
|--------|-------------------|
| デジットシンボルマッチング | TMB Digit Symbol Matching |
| タップして続ける | (button label — this part is translated) |
| ― | Skip practice trials（未翻訳） |
| ― | View practice trials（未翻訳） |

---

## 8. 完了画面 / Completion Screens

GradCPTと同じ2パターンの完了分岐（`practiceonly`相当の仕組みはDSM原版に存在しないため，未使用パターンは無い）。
Two completion paths, matching GradCPT's structure (DSM's original code has no `practiceonly`-equivalent, so there is no unused legacy path here).

### 8-1. 通常の本番完了（cognitive.html経由，firstrun未指定） / Standard main-session completion

| 日本語 | English (Original) |
|--------|-------------------|
| 課題が完了しました。<br>ありがとうございました。<br>自動的に画面が切り替わります… | Your score is X.<br>The test is over.<br>Thank you for participating!（原文を簡略化・GradCPTと体裁統一） |

完了後，GASへ集計・詳細データを送信し，3秒後に`cognitive.html`へ自動遷移する。
Sends summary/detail data to GAS, then auto-redirects to `cognitive.html` after 3 seconds.

### 8-2. 練習ページでの実施完了（firstrun=true，現在使用中） / Practice-page completion (firstrun=true, currently active)

| 日本語 | English (Original) |
|--------|-------------------|
| DSMの練習課題が完了しました！<br>お疲れさまでした。<br>続けて2-backタスクの練習に進みます… | （追加機能：原文なし / Added feature: no original） |

GASへのデータ送信は行わない。完了フラグをローカル保存し，3秒後に`practice.html?step=3`（2-back練習ステップ）へ自動遷移する。
No data is sent to GAS. A local completion flag is stored, then auto-redirects to `practice.html?step=3` (the 2-back practice step) after 3 seconds.

---

## 付記：URLパラメータ / URL Parameters

DSM原版の`URL params`シート（TMB_DSMDictionary_v1_Jul24.xlsx）に基づく。GradCPTとはパラメータ体系が異なる点に注意（刺激ファイルではなく`seed`で刺激パターンを制御）。
Based on the original `URL params` sheet (TMB_DSMDictionary_v1_Jul24.xlsx). Note the parameter scheme differs from GradCPT — stimulus pattern is controlled via `seed`, not a stimulus file.

| パラメータ | 説明 | 状態 |
|-----------|------|------|
| `seed` | 乱数シード。刺激パターン（シンボル-数字の組み合わせ順序）を決定 | 使用中（練習ページはseed=990001固定） |
| `duration` | テストの制限時間（秒），既定90秒 | 未指定（既定値90秒をそのまま使用） |
| `nopractice` | 練習のスキップ設定（true/false/optional） | 使用予定（本番Day2〜14でtrue，GradCPTと同様の想定） |
| `moresymbols` | 30種のシンボルプールから抽出するか（false=標準6種） | 未指定（既定のfalse＝標準6種を使用） |
| `chooseinput` | タップ/キーボード選択UI（chooseInput.js）を使うか | 使用中（常にfalseを指定し，英語UIを回避） |
| `firstrun` | 練習課題ページでの実施であることを示す（本研究で追加。GAS送信を抑止し，完了後は次の練習ステップへ遷移） | **使用中**（practice.html専用） |
| `demo` | デモモード（10秒のみのテスト） | 未使用 |

### 使用例 / Usage Examples

```
# 本番（Day 1，練習あり・cognitive.html未実装のためTBD，seed値も未定）
DSM_Main.v1.Jul24.html?seed=[TBD]&chooseinput=false

# 本番（Day 2〜14，練習なし・cognitive.html未実装のためTBD）
DSM_Main.v1.Jul24.html?seed=[TBD]&nopractice=true&chooseinput=false

# 練習課題ページでの実施（practice.htmlから実際に呼び出している形式）
DSM_Main.v1.Jul24.html?seed=990001&firstrun=true&chooseinput=false
```

上記のうち「本番」の呼び出し例は，`cognitive.html`実装時に確定する想定（現時点ではTBD）。Day1〜14で使用するseed値は，GradCPTのpicsInput_day01〜14.txtに相当する仕組みとして，別途決定が必要。
The "main session" examples above are provisional; the final form, including the Day1–14 seed values (analogous to GradCPT's picsInput_day01–14.txt files), will be confirmed when `cognitive.html` is implemented.
