# GradCPT 日英テキスト対照表
# Japanese–English Text Reference for GradCPT (EMA Version)
#
# 最終更新 / Last updated: 2026-08-11
# 対象ファイル / Source file: GradCPT_Main.v1.Apr24.html
#
# 原典 / Source:
#   TestMyBrain GradCPT (Gradual Onset Continuous Performance Test)
#   The Many Brains Project (manybrains.net) — GNU LGPLv3
#   Original task: Esterman et al. (2013); Rosenberg et al. (2013)
#
# 本研究での修正内容 / Modifications for this study:
#   - 300試行（標準版）→ 75試行（EMA版）
#   - 標的（都市）: 89.3% → 80%，非標的（山）: 10.7% → 20%
#   - 全テキストを日本語化
#   - 14日分の異なる刺激順序ファイル（本番）＋練習専用ファイル1本を使用
#   - 試行完了後にGASへデータを自動送信（練習ページでの実施を除く）
#   - Standard 300 trials → EMA 75 trials
#   - Target (city): 89.3% → 80%, Non-target (mountain): 10.7% → 20%
#   - All UI text translated to Japanese
#   - 14 daily stimulus sequence files + 1 dedicated practice-only file
#   - Auto-submit results to GAS on completion (except when run from practice.html)
#
# 参照 / Reference:
#   Hawks et al. (2024). npj Digital Medicine, 7, 59.
#   https://doi.org/10.1038/s41746-024-01036-5
#
# 用語について / Note on terminology:
#   本ファイルにおいて「本番」は，研究1トップページの「今日の認知課題」
#   （cognitive.html）経由で毎日実施するデータ収集セッションのみを指す。
#   練習課題ページ（practice.html）で実施する内容（75試行テストを含む）は
#   すべて「練習」であり，参加者向けの文言にも「本番」という語は使用しない。
#   "本番" (main/production session) refers exclusively to the daily data-
#   collection session via cognitive.html. Everything run from practice.html,
#   including its full 75-trial test, is "practice," and participant-facing
#   text never uses the word "本番" for it.

---

## 1. タイトル画面 / Title Screen

| 日本語 | English (Original) |
|--------|-------------------|
| 集中力課題 | Continuous Concentration |

---

## 2. 説明画面 / Instruction Screen

| 日本語 | English (Original) |
|--------|-------------------|
| 説明 | Instructions |
| これから**山**と**街**の写真が次々と表示されます。 | You will see pictures of mountains and cities. |

---

## 3. 練習説明 / Practice Instructions

practice1・practice3・practice5の3箇所で同一テキストパターンを使用（練習パートが進むごとに繰り返し表示）。
Used identically at practice1, practice3, and practice5 (repeated as the practice stages progress).

### (タップ版 / Touch version)

| 日本語 | English (Original) |
|--------|-------------------|
| 説明：（practice1のみ）/ 課題は同じです：（practice3・practice5） | Instructions: / The task is the same: |
| **街**の写真が表示されたら，できるだけ早く**タップ**してください。 | When you see a **CITY** picture, **tap it** as quickly as you can. |
| **山**の写真が表示されたら，**タップしないでください。** | When you see a **MOUNTAIN** picture, **DON'T TAP** it. |
| 練習してみましょう。 | Let's practice. |

### (キーボード版 / Keyboard version)

| 日本語 | English (Original) |
|--------|-------------------|
| **街**の写真が表示されたら，できるだけ早く**スペースキー**を押してください。 | When you see a **CITY** picture, press and release the **SPACE BAR** as quickly as you can. |
| **山**の写真が表示されたら，**何も押さないでください。** | When you see a **MOUNTAIN** picture, **DON'T PRESS** any key. |

---

## 4. 練習移行メッセージ / Practice Transition Messages

| # | 日本語 | English (Original) |
|---|--------|-------------------|
| 練習2移行（practice2） | よくできました！次のパートでは，写真がフェードしながら次々と切り替わります。途中で止まりません。 | Good! For the next part of the practice, the pictures will fade from one to the next without pausing. |
| 練習4移行（practice4） | よくできました！最後の練習パートでは，写真がさらに速く切り替わります。フィードバックは表示されません。 | Great! For the final part of the practice, the pictures will alternate faster and there will be no feedback. |
| テスト前（practice6） | よくできました！次にテストを行います。フィードバックは表示されません。テストは約X分間続きます。集中して取り組んでください。 | Excellent! Next, we'll start the task. We will not give you any feedback. The activity will only last X minutes. |

**2026-08-11修正：** 「テスト前」メッセージは元々「次に**本番**の課題を始めます」という文言だったが，練習ページでの実施は本番ではないため「次に**テスト**を行います」に修正。
**2026-08-11 fix:** The pre-test message previously said "next, we'll start the **main task** (本番)," which was corrected to "next, we'll do the **test** (テスト)," since execution on the practice page is never the main/production session.

---

## 5. テスト直前の確認メッセージ / Pre-Test Reminder（test1）

### (タップ版 / Touch version)

| 日本語 | English (Original) |
|--------|-------------------|
| 確認： | Remember: |
| **街**の写真 → **タップ** | When you see a **CITY** picture **tap it** as quickly as you can. |
| **山**の写真 → **タップしない** | When you see a **MOUNTAIN** picture **DON'T TAP** it. |
| それでは始めましょう。 | Let's start the test. |

---

## 6. 練習フィードバック（practice1個別試行） / Practice Feedback (practice1 per-trial)

| 日本語 | English (Original) |
|--------|-------------------|
| 正解！ | Correct! |
| 不正解。<br>山には反応しないでください。 | Incorrect!<br>You do not respond to mountains! |
| 反応が遅すぎました。<br>街の写真をタップしてください！（タップ版） | You took too long to respond.<br>You must tap city pictures! |
| 反応が遅すぎました。<br>街の写真が出たらスペースキーを押してください。（キーボード版） | You took too long to respond.<br>You must press and release the space bar |
| タップしてやり直す（再試行ボタン） | (retry button, added for this study) |

---

## 7. 画面遷移ボタン文言 / Continue / Advance Button Labels

begin・messageタイプのフレーム（各説明画面）で共通して使用。
Used across all "begin" and "message" type frames (instructional screens).

| 画面 | タップ版 | キーボード版 |
|------|---------|------------|
| 冒頭の説明へ進む（begin） | タップして説明を見る | スペースキーを押して説明を見る |
| 通常の「続ける」（message） | タップして続ける | クリック / スペースキーで続ける |

---

## 8. 練習スキップ画面 / Practice Skip Screen（nopractice=optional時のみ）

**現在未使用：** 本研究のURL呼び出しでは`nopractice`を`'optional'`に設定することがないため，このスキップ選択画面自体を参加者が目にすることはない。ラジオボタンの選択肢テキストは未翻訳のまま（英語）で残っている。
**Currently unused:** This study's URL calls never set `nopractice` to `'optional'`, so participants never see this screen. Its radio-button option text remains untranslated (English).

| 日本語 | English (Original / 現状のまま未翻訳) |
|--------|-------------------|
| 集中力課題 | TMB Continuous Performance |
| タップして続ける | (button label — this part is translated) |
| ― | Skip instructions & practice trials（未翻訳） |
| ― | View instructions & practice trials（未翻訳） |

---

## 9. 完了画面 / Completion Screens

本研究での改修により，完了時の分岐が3パターンに増えている。
Three completion paths now exist as a result of this study's modifications.

### 9-1. 通常の本番完了（cognitive.html経由，firstrun未指定） / Standard main-session completion

| 日本語 | English (Original) |
|--------|-------------------|
| 課題が完了しました。<br>ありがとうございました。<br>自動的に画面が切り替わります… | Your score is X. The test is over. Thank you for participating!（原文を簡略化・体裁統一） |

完了後，GASへ集計・詳細データを送信し，3秒後に`cognitive.html`へ自動遷移する。
Sends summary/detail data to GAS, then auto-redirects to `cognitive.html` after 3 seconds.

### 9-2. 練習ページでの実施完了（firstrun=true，現在使用中） / Practice-page completion (firstrun=true, currently active)

| 日本語 | English (Original) |
|--------|-------------------|
| GradCPTの練習課題が完了しました！<br>お疲れさまでした。<br>続けてDSM（デジットシンボルマッチング）の練習に進みます… | （追加機能：原文なし / Added feature: no original） |

GASへのデータ送信は行わない。完了フラグをローカル保存し，3秒後に`practice.html?step=2`（DSM練習ステップ）へ自動遷移する。
No data is sent to GAS. A local completion flag is stored, then auto-redirects to `practice.html?step=2` (the DSM practice step) after 3 seconds.

### 9-3. 練習のみモード完了（practiceonly=true，現在未使用のレガシー機能） / Practice-only mode completion (practiceonly=true, legacy/unused)

| 日本語 | English (Original) |
|--------|-------------------|
| GradCPTの練習が完了しました！<br>（タップ版）タップして次の課題へ進む<br>（キーボード版）クリック / スペースキーで次の課題へ進む | （追加機能：原文なし / Added feature: no original） |

**2026-08-11時点で未使用：** `practiceonly=true`は「練習トライアルのみ実施し，75試行テストを省略する」機能で，過去のバージョンではpractice.htmlから呼び出していたが，現在は9-2の`firstrun=true`方式に置き換えられている。コードは後方互換のため残しているが，実際のURL呼び出しでは使用しない。
**Unused as of 2026-08-11:** `practiceonly=true` skips the 75-trial test and shows practice-only completion. It was previously called from practice.html but has been superseded by the `firstrun=true` approach in 9-2. The code remains for backward compatibility but is not used in any current URL call.

---

## 付記：URLパラメータ / URL Parameters

| パラメータ | 説明 | 状態 |
|-----------|------|------|
| `input` | 刺激リストファイルの指定 | 使用中 |
| `nopractice` | 練習のスキップ設定（true/false/optional） | 使用中（本番Day2〜14でtrue） |
| `chooseinput` | タップ/キーボード選択UI（chooseInput.js）を使うか | 使用中（常にfalseを指定し，英語UIを回避） |
| `firstrun` | 練習課題ページでの実施であることを示す（本研究で追加。GAS送信を抑止し，完了後は次の練習ステップへ遷移） | **使用中**（practice.html専用） |
| `practiceonly` | 練習のみ実施し75試行テストを省略（本研究で追加） | **未使用（レガシー）** |
| `seed` | 乱数シード | 未使用（GradCPTは`input`ファイルで刺激順序を指定するため） |

### 使用例 / Usage Examples

```
# 本番（Day 1，練習あり・cognitive.html未実装のためTBD）
GradCPT_Main.v1.Apr24.html?input=picsInput_75imgs_15nogo_day01.txt&chooseinput=false

# 本番（Day 2〜14，練習なし・cognitive.html未実装のためTBD）
GradCPT_Main.v1.Apr24.html?input=picsInput_75imgs_15nogo_day02.txt&nopractice=true&chooseinput=false

# 練習課題ページでの実施（practice.htmlから実際に呼び出している形式）
GradCPT_Main.v1.Apr24.html?input=picsInput_75imgs_15nogo_practice.txt&firstrun=true&chooseinput=false
```

上記のうち「本番」の呼び出し例は，`cognitive.html`実装時に確定する想定（現時点ではTBD）。
The "main session" examples above are provisional; the final form will be confirmed when `cognitive.html` is implemented.
