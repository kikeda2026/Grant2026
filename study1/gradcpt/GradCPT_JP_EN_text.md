# GradCPT 日英テキスト対照表
# Japanese–English Text Reference for GradCPT (EMA Version)
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
#   - 14日分の異なる刺激順序ファイルを使用
#   - 試行完了後にGASへデータを自動送信
#   - Standard 300 trials → EMA 75 trials
#   - Target (city): 89.3% → 80%, Non-target (mountain): 10.7% → 20%
#   - All UI text translated to Japanese
#   - 14 different stimulus sequence files (one per day)
#   - Auto-submit results to GAS on completion
#
# 参照 / Reference:
#   Hawks et al. (2024). npj Digital Medicine, 7, 59.
#   https://doi.org/10.1038/s41746-024-01036-5

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
### (タップ版 / Touch version)

| 日本語 | English (Original) |
|--------|-------------------|
| 説明： | Instructions: |
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
| 練習2移行 | よくできました！次のパートでは，写真がフェードしながら次々と切り替わります。途中で止まりません。 | Good! For the next part of the practice, the pictures will fade from one to the next without pausing. |
| 練習4移行 | よくできました！最後の練習パートでは，写真がさらに速く切り替わります。フィードバックは表示されません。 | Great! For the final part of the practice, the pictures will alternate faster and there will be no feedback. |
| 本番前 | よくできました！次に本番の課題を始めます。フィードバックは表示されません。課題は約X分間続きます。集中して取り組んでください。 | Excellent! Next, we'll start the task. We will not give you any feedback. The activity will only last X minutes. |

---

## 5. 本番確認メッセージ / Pre-Test Reminder
### (タップ版 / Touch version)

| 日本語 | English (Original) |
|--------|-------------------|
| 確認： | Remember: |
| **街**の写真 → **タップ** | When you see a **CITY** picture **tap it** as quickly as you can. |
| **山**の写真 → **タップしない** | When you see a **MOUNTAIN** picture **DON'T TAP** it. |
| それでは始めましょう。 | Let's start the test. |

---

## 6. 練習フィードバック / Practice Feedback

| 日本語 | English (Original) |
|--------|-------------------|
| 正解！ | Correct! |
| 不正解！ | Incorrect! |

---

## 7. エラーメッセージ / Error Messages

| 日本語 | English (Original) |
|--------|-------------------|
| 反応が遅すぎました。 | You took too long to respond. |
| 街の写真をタップしてください！ | You must tap city pictures! |
| 街の写真が出たらスペースキーを押してください | You must press and release the space bar |
| タップして説明を見る | Tap here for instructions |
| スペースキーを押して説明を見る | Press the SPACEBAR for instructions |
| 山には反応しないでください。 | You do not respond to mountains! |

---

## 8. 練習スキップ画面 / Practice Skip Screen

| 日本語 | English (Original) |
|--------|-------------------|
| 集中力課題 | TMB Continuous Performance |
| 説明と練習をスキップして始める | Skip instructions & practice trials |
| 説明と練習を行ってから始める | View instructions & practice trials |

---

## 9. 完了画面 / Completion Screen

| 日本語 | English (Original) |
|--------|-------------------|
| 課題が完了しました。ありがとうございました。自動的に画面が切り替わります… | Your score is X. The test is over. Thank you for participating! |

---

## 10. 練習専用モード完了 / Practice-Only Mode Completion

| 日本語 | English (Original) |
|--------|-------------------|
| GradCPTの練習が完了しました！次の課題の練習へ進みます… | （追加機能：原文なし / Added feature: no original） |

---

## 付記：URLパラメータ / URL Parameters

| パラメータ | 説明 | 例 |
|-----------|------|-----|
| `input` | 刺激リストファイルの指定 | `input=picsInput_75imgs_15nogo_day01.txt` |
| `nopractice` | 練習のスキップ設定 | `nopractice=true` |
| `practiceonly` | 練習のみ実施（本研究で追加） | `practiceonly=true` |
| `seed` | 乱数シード | `seed=1` |

### 使用例 / Usage Examples

```
# 本番（Day 1，練習あり）
GradCPT_Main.v1.Apr24.html?input=picsInput_75imgs_15nogo_day01.txt

# 本番（Day 2〜14，練習なし）
GradCPT_Main.v1.Apr24.html?input=picsInput_75imgs_15nogo_day02.txt&nopractice=true

# 練習専用モード（practice.htmlから呼び出し）
GradCPT_Main.v1.Apr24.html?input=picsInput_75imgs_15nogo_day01.txt&practiceonly=true
```
