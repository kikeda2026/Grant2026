# 認知課題に関する研究計画書（プレレジ草稿）

**研究課題：** 運動による血糖値変動の安定化が認知機能を介してうつ状態の改善に至る因果的媒介過程の検証  
**作成日：** 令和8年8月  
**バージョン：** 第1版（認知課題仕様確定前の暫定版）

> **注記：** 本文書は，認知課題（GradCPT・DSM・2-backの3課題）の仕様が確定し次第，具体的なパラメータ（試行数・提示時間等）を補完して最終版とする予定である。本文中の `[TBD]` は今後確定する事項を示す。

---

## 1. 研究背景：認知課題選択の理論的根拠

### 1.1 血糖値変動と認知機能の関連

近年，血糖値の変動幅（glycemic variability; GV）が認知機能に対して有害な影響を及ぼすことが，複数の研究から示されている。[Banks et al.（2018）](#banks-et-al-2018)は，インスリンが血液脳関門を通過し，海馬や前頭前皮質における神経可塑性・シナプス伝達に直接関与することを示した。食後の急激な血糖上昇・下降（血糖値スパイク）は，これらの脳領域での代謝的ストレスを高め，一時的な認知機能の低下をもたらす可能性がある。

特に重要な知見として，[Hawks et al.（2024）](#hawks-et-al-2024)は，持続血糖モニター（CGM）と認知的EMAを組み合わせた研究において，**日常生活における自然発生的な血糖変動が処理速度（processing speed）の低下と動的に関連すること**を，1型糖尿病患者において実証した。この研究は，血糖変動と認知機能の関係が実験室環境にとどまらず，日常的な生活場面においても観察されることを示した点で方法論的に重要であり，本研究の設計（CGM＋認知的EMA）の妥当性を直接支持する。

血糖値変動とうつ状態の関連については，[Kim et al.（2022）](#kim-et-al-2022)が糖尿病のない一般韓国人集団において，空腹時血糖の変動指標が大きいほど抑うつリスクが有意に高まることを，後ろ向きコホート研究により示した。同様に，[Kwon et al.（2023）](#kwon-et-al-2023)は長期的な血糖値変動が抑うつ障害および不安障害のリスクと有意に関連することを報告している。これらの知見は，血糖値変動→認知機能→うつ状態という媒介経路の存在を示唆する疫学的証拠を提供するものである。さらに，認知機能とうつ状態の関係は双方向的であることが示されており，[Yin et al.（2024）](#yin-et-al-2024)は大規模縦断データを用いて，抑うつ症状と認知機能が時間的に相互に影響を与え合うことを明らかにした。この双方向性は，本研究の媒介モデルの中で認知機能を中心的な連結変数として位置づける理論的根拠を強化するものである。

注意の持続（sustained attention），処理速度（processing speed），およびワーキングメモリ（working memory）は，血糖値変動の影響を受けやすい認知領域として位置づけられているが（[Yu et al., 2020](#yu-et-al-2020); [Schaich et al., 2024](#schaich-et-al-2024)），認知領域間で感受性の差異が存在することも示されている。[Hawks et al.（2024）](#hawks-et-al-2024)はCGM＋認知的EMAを用いた最初の大規模研究において，3種類の認知課題（処理速度：デジットシンボルマッチング，持続的注意：GradCPT，ワーキングメモリ：MOT）を毎日複数回測定した結果，**血糖変動が処理速度とは動的に関連する一方，持続的注意とは有意な関連を示さなかった**と報告した。この知見は，処理速度が血糖変動の認知的影響を捉える上で最も感受性の高い指標であることを示唆する。一方，別の研究では夜間の血糖変動の大きさが翌日の持続的注意の低下を予測することも報告されており，持続的注意課題が血糖変動の遅延効果の指標として機能する可能性は否定されない。ワーキングメモリについては，インスリン感受性と脳内グルコース代謝を介した関連が確認されており（[Banks et al., 2018](#banks-et-al-2018)），海馬依存的な情報の一時保持・更新プロセスが血糖値変動の影響に対して感受性が高いことが報告されている。

なお，認知機能の低下とうつ状態の関連についても先行研究の裏づけがある。[Formánek et al.（2020）](#formánek-et-al-2020)は抑うつ症状の軌跡と認知機能低下のパターンが関連することを示し，認知機能の変化がうつ状態の推移を予測しうることを報告している。

### 1.2 繰り返し測定アプローチとしてのEMAの有効性

認知機能の日内・日間変動を捉えるためには，従来の実験室に基づく横断的な測定では限界がある。日常生活場面における認知機能の変動を繰り返し・リアルタイムに測定する手法として，Ecological Momentary Assessment（EMA）を応用したモバイル認知課題が近年注目されている（[Sliwinski et al., 2018](#sliwinski-et-al-2018)）。

本研究に最も近い先行研究として，[Hawks et al.（2024）](#hawks-et-al-2024)は，CGMと認知的EMAを組み合わせた初の大規模研究を実施し，1型糖尿病患者における**日常的な血糖変動と処理速度の動的関連**を実証した。この研究は，実験室での急性血糖負荷実験ではなく，日常生活の中で自然に生じる血糖変動が認知パフォーマンスに影響を与えることを初めて定量的に示したものであり，本研究の方法論的枠組みの直接的な先例となる。

[Zlatar et al.（2022）](#zlatar-et-al-2022)は，多様な健康状態を持つ成人90名を対象に，スマートフォンを用いた認知課題を1日2回，14日間実施する研究を行い，参加者のアドヒアランスが高く（13/14日以上の完了率），身体活動と実行機能の日内変動を捉えることに成功したことを報告している。また，[Campbell et al.（2020）](#campbell-et-al-2020)は，中高年成人103名において，モバイル認知課題による1日4回・14日間の繰り返し測定が実現可能であることを示し，日常活動と認知機能の動的な関連を明らかにした。

スマートウォッチを用いた1-backタスクを1日4回・7日以上実施した研究では，課題のアドヒアランス率が78%を超え，課題の信頼性は4〜6試行後に安定し，5ヶ月後の再検査信頼性も良好であることが確認されている（[Schmitter-Edgecombe et al., 2024](#schmitter-edgecombe-et-al-2024)）。これらの知見は，モバイルデバイスを用いた日々の認知測定が，方法論的に妥当かつ実用的であることを支持する。

### 1.3 繰り返し測定における練習効果への対処

認知課題を繰り返し実施する際に懸念される主要な方法論的問題は，練習効果（practice effects; PE）である。[Falleti et al.（2006）](#falleti-et-al-2006)は，健常若年成人（18〜40歳，45名）を対象に，コンピュータ化認知バッテリー（CogState）を10分間隔で4回，その後1週間後にも実施した研究において，成績は第1回から第2回にかけて有意に向上し（練習効果が最大），**第2回以降では成績が安定する**ことを報告した。すなわち，毎日測定を行う縦断的研究においては，練習効果は主として初期の数回に集中し，以降の測定では安定した成績が期待できる。

この知見は，本研究のような14日間の毎日測定において，**実質的な練習効果は測定初日から数日以内に収束する**ことを示唆している。同様に，[Schmitter-Edgecombe et al.（2024）](#schmitter-edgecombe-et-al-2024)は，EMAによるNバック課題において練習効果そのものを認知指標として位置づける視点を提示しており，**練習効果の欠如が認知機能低下のマーカーとなりうる**可能性も指摘している。

以上の先行研究を踏まえ，本研究では以下の方略を採用することで，練習効果を適切に管理する。

1. **練習試行の実施：** 本番前に十分な数の練習試行を設け，課題手順への慣れを促す
2. **ウォームアップ期間の設定：** [Falleti et al.（2006）](#falleti-et-al-2006)が示すとおり，成績は第2回目以降で安定することから，**初日（第1回）のみ**を「慣れ期間」として扱い，分析モデルにおいて共変量として統制する。また，データ取得後に個人内の学習曲線に対して混合効果モデルを適用し，成績が安定し始める日を経験的に同定する**事後的感度分析**も実施する。これにより，慣れ期間の設定の妥当性を透明な形で検証する。
3. **刺激のランダム化：** 毎回異なる刺激順序・刺激セットを使用し，特定刺激への慣れを防ぐ

---

## 2. 研究仮説

本研究では，認知課題に関して以下の仮説を設定する。

### 2.1 主要仮説

**仮説1（研究1）：** 血糖値変動指標（例：MAGE，標準偏差）が大きい日は，翌日または同日の**処理速度**（DSM反応時間）が低下する（血糖値変動→処理速度への日内変動効果）。本仮説は[Hawks et al.（2024）](#hawks-et-al-2024)の知見に基づく最も強い先験的予測である。

**仮説2（研究1）：** 血糖値変動指標が大きい日は，翌日または同日の**ワーキングメモリ成績**（2-back *d'*・反応時間）が低下する（血糖値変動→ワーキングメモリへの日内変動効果）。

**仮説3（研究1）：** 血糖値変動指標が大きい日は，翌日の**持続的注意**（GradCPT *d'*）が低下する（血糖値変動の遅延効果）。本仮説は急性効果よりも蓄積効果を想定した探索的な位置づけとする。

**仮説4（研究1）：** 上記の認知機能の日内変動は，抑うつ傾向（CES-D得点）の変化と関連する（認知機能→気分状態の時系列的関連）。

**仮説5（研究2）：** 運動介入群では，対照群と比較して，血糖値変動が安定し，かつ認知課題成績（GradCPT・DSM・2-back）が改善する（運動介入の直接効果）。

**仮説6（研究2）：** 運動介入の抗うつ効果は，血糖値変動の安定化および認知機能の改善を介して媒介される（間接効果：運動→血糖値変動→認知機能→うつ状態）。

### 2.2 探索的仮説

**探索的仮説1：** 練習効果の収束速度（すなわち，課題成績が安定するまでの試行数）は，血糖値変動の大きさと負の相関を示す（血糖値変動が大きい参加者ほど練習効果が遅延する）。

**探索的仮説2：** 認知課題成績の個人内変動量（intraindividual variability; IIV）は，血糖値変動指標と正の相関を示す。

---

## 3. 認知課題の手続き

### 3.1 概要

本研究の認知課題はスマートフォンまたはPCのWebブラウザ上で動作するプログラムを用いて実施する。参加者は研究期間（14日間）中，毎日夕食後60〜90分以内に以下の3課題を連続して行う。

| 課題 | 測定領域 | 所要時間（目安） |
|------|---------|--------------|
| Gradual Onset CPT（GradCPT） | 持続的注意 | 約1分 |
| デジットシンボルマッチング（DSM） | 処理速度 | 約1.5分 |
| 2-backタスク | ワーキングメモリ | 約3〜5分 |

**1日あたりの合計実施時間：約6〜8分**（従来の10分/課題設計を大幅に短縮）

この設計は[Hawks et al.（2024）](#hawks-et-al-2024)およびGluCog研究（[Chaytor et al., 2023](#chaytor-et-al-2023)）のEMA認知課題設計に基づく。GradCPTは75試行・800ミリ秒/試行で所要時間は約60秒，DSMは約90秒として設計されており，本研究も同一の設計思想を採用する。

#### 実施順序

毎日の3課題の提示順序は乱数を用いてランダムに決定する。これにより，14日間の測定にわたって順序効果が統計的に相殺される。

---

### 3.2 Gradual Onset Continuous Performance Test（GradCPT）

#### 3.2.1 課題の目的と測定構成概念

GradCPTは持続的注意（sustained attention）および抑制制御（inhibitory control）を測定する課題である。従来のCPT-X形式（突然の刺激提示）と異なり，GradCPTでは刺激が徐々にフェードイン・フェードアウトする設計を採用しており，外因性注意捕捉（刺激の急激な出現による反射的注意）の影響を最小化し，内発的・持続的な注意制御をより純粋に測定できる（[Hawks et al., 2024](#hawks-et-al-2024)）。本課題は[Hawks et al.（2024）](#hawks-et-al-2024)のGluCog研究においてCGM＋EMAデザインで使用・検証済みである。

#### 3.2.2 刺激と提示条件

- **刺激種類：** 都市（city）または山（mountain）のグレースケール画像
- **標的刺激：** 都市画像（全試行の80%）
- **非標的刺激：** 山画像（全試行の20%）
- **提示方式：** 各試行間でフェードイン・フェードアウト（800ミリ秒/試行）
- **試行数：** 本番 **75試行**（所要時間：約60秒），練習 [TBD] 試行
- **刺激提示順序：** 毎回ランダム化

#### 3.2.3 反応方法

都市画像が提示された際（標的）に画面タップまたはキー押しで反応し，山画像（非標的）には反応を抑制する。反応時間はミリ秒単位で計測する。

#### 3.2.4 測定指標

| 指標 | 説明 | 算出方法 |
|------|------|---------|
| **感度指標（*d'*）** | 標的検出の感受性を示す信号検出理論的指標 | *d'* = Z(Hit rate) - Z(False alarm rate) |
| **正答率（Hit rate）** | 標的が出現したときに正しく反応した割合 | 正反応数 / 標的呈示数 |
| **誤反応率（False alarm rate）** | 非標的に対して誤って反応した割合 | 誤反応数 / 非標的呈示数 |
| **反応時間（RT）** | 正反応試行における反応時間中央値（ms） | 正反応試行のRTの中央値 |

主要な分析指標は *d'* とする。

---

### 3.3 デジットシンボルマッチング（Digit Symbol Matching; DSM）

#### 3.3.1 課題の目的と測定構成概念

DSMは処理速度（processing speed）を測定する課題である。処理速度とは，単純な情報を素早く正確に処理する能力であり，前頭線条体ネットワークが関与する。[Hawks et al.（2024）](#hawks-et-al-2024)において，3つの認知領域（処理速度・持続的注意・ワーキングメモリ）のうち**血糖値変動と最も動的な関連を示した唯一の認知領域**であり，本研究における主要測定指標として位置づける。

#### 3.4.2 刺激と提示条件

- **課題形式：** 数字（1〜9）とシンボルの対応表を参照しながら，提示された数字に対応するシンボルを選択する
- **試行数：** 本番 [TBD] 試行（所要時間：約90秒），練習 [TBD] 試行
- **対応表：** 毎回ランダムに異なる数字-シンボル対応を使用し，記憶による練習効果を防ぐ

#### 3.4.3 反応方法

画面に提示された対応表を参照し，標的シンボルを選択肢の中からタップする。

#### 3.4.4 測定指標

| 指標 | 説明 |
|------|------|
| **正答数（Correct responses）** | 制限時間内に正しく回答した試行数（主要指標） |
| **反応時間（RT）** | 正反応試行の反応時間中央値（ms） |
| **正答率（Accuracy）** | 全試行に占める正答の割合 |

---

### 3.4 2-backタスク（ワーキングメモリ）

#### 3.4.1 課題の目的と測定構成概念

Nバック課題はワーキングメモリ（working memory）を測定する課題である。ワーキングメモリとは，情報を一時的に保持しながら同時に別の認知処理を行う能力であり，学習・問題解決・感情制御の基盤となる（[Brose et al., 2012](#brose-et-al-2012)）。本課題では，現在提示されている刺激が *N* 個前の刺激と同一であるかを判断する。本研究では**2-backのみ**を実施する。

#### 3.4.2 刺激と提示条件

- **刺激種類：** アルファベット大文字（A〜Z の中から [TBD] 文字を使用）
- **標的条件：** 現在の刺激が *N* 個前の刺激と同一
- **標的出現率：** 全試行の約25〜33%
- **刺激提示時間：** [TBD] ミリ秒
- **刺激間隔（ISI）：** [TBD] ミリ秒
- **実施難易度：** 2-back（[TBD]試行）のみ実施する。1-backは健常成人では天井効果が生じやすく，血糖値変動の効果量を捉えにくい。2-backは前頭前皮質（DLPFC）の活性化を強く必要とし，健常成人において床効果・天井効果を回避できる難易度として先行研究で最も広く採用されている（[Lezak et al., 2004](#lezak-et-al-2004); [Kirchner, 1958](#kirchner-1958)）。
- **刺激提示順序：** 毎回ランダム化

#### 3.4.3 反応方法

標的刺激が提示されたと判断した場合は，スマートフォンでは画面タップ，PCではスペースキーを押す。標的でない場合は反応しない。

#### 3.4.4 測定指標

| 指標 | 説明 | 算出方法 |
|------|------|---------|
| **感度指標（*d'*）** | 信号検出理論に基づく検出感度 | *d'* = Z(Hit rate) - Z(False alarm rate) |
| **正答率（Hit rate）** | 標的試行での正反応率 | 正反応数 / 標的試行数 |
| **誤反応率（False alarm rate）** | 非標的試行での誤反応率 | 誤反応数 / 非標的試行数 |
| **反応時間（RT）** | 正反応試行の反応時間中央値（ms） | 正反応試行のRTの中央値 |
| **個人内変動量（IIV）** | 14日間の成績変動の標準偏差 | SD of daily *d'* scores |

1-backと2-backの成績はそれぞれ独立した指標として分析するとともに，2つを合成した複合スコアの使用も検討する。

---

### 3.5 実施手順の詳細

#### 3.5.1 初回セッション（初日）

初日の実験開始時に，研究担当者が以下の手順を参加者に説明する。

1. **課題の説明：** 各課題（GradCPT・DSM・2-back）の目的・手順・反応方法をWeb上の説明ページおよび口頭で説明する
2. **練習試行：** 3課題それぞれについて十分な数の練習試行を実施する。参加者が課題の意味を正しく理解したことを確認してから本番に進む
3. **本番試行（1日目データ収集開始）**

#### 3.5.2 2日目以降（毎日）

- 毎日，できるだけ同じ時間帯（参加者が設定する時間帯）に課題を実施する
- スマートフォンまたはPCのブラウザから研究専用ページにアクセスし，参加者IDを入力して課題に取り組む
- 実施前に体調を確認する。著しく体調が悪い場合は無理に実施しないよう案内する。【**保留：実施するかどうか検討中**】
- 課題実施後，データは自動でサーバーに送信される

#### 3.5.3 実施時刻の設定根拠

本研究では，**夕食後60〜90分以内**を毎日の認知課題の実施時刻として設定する。この設定の根拠は以下の通りである。

食後の血糖値は摂取後30〜60分でピークに達し，60〜90分以降に緩やかに低下する（late postprandial period）。[Nilsson et al.（2012）](#nilsson-et-al-2012)は，高GI食と低GI食の比較において，食後90分時点でのワーキングメモリ成績（*P* = .034）および170分時点での選択的注意成績（*P* = .017）に有意差が認められたことを示した。また，[Ingwersen et al.（2012）](#ingwersen-et-al-2012)は，食後75〜225分の後期食後段階において，GI値の低い朝食摂取後に選択的注意が有意に改善したことを報告している。

これらの知見は，**血糖値変動が認知機能に与える影響は食後60分以降の後期食後段階において最も検出可能**であることを示唆する。一方，食後30分以内の急峻な血糖上昇期は，消化に伴う血流再配分や眠気により認知課題への集中が困難となり，データの信頼性が低下する可能性がある。

夕食を選択する理由は，一般に夕食後の血糖値の上昇は朝食後よりも高く，夕方の食事が食後高血糖状態を悪化させることが健常成人において実証されているため（[Takahashi et al., 2018](#takahashi-et-al-2018)），夕食後が血糖変動の認知機能への影響を測定する感度が高いと考えられるからである。実施時刻はデータに自動記録し，分析モデルの共変量として投入する。

---

### 3.6 データの記録・管理

各試行の以下のデータがサーバー（Google スプレッドシート）に自動記録される。

- 参加者ID
- 実施日時（タイムスタンプ）
- 課題種別（GradCPT / DSM / 2-back）
- 試行番号
- 刺激の種類（標的 / 非標的）
- 提示刺激（アルファベット文字）
- 参加者の反応（有 / 無）
- 反応時間（ミリ秒）
- 正誤判定

これらの試行レベルデータを用いて，日次の *d'*，正答率，誤反応率，反応時間中央値，および14日間の個人内変動量（IIV）を算出する。

---

### 3.7 除外基準

以下の基準に該当する試行・セッションは分析から除外する。

- 反応時間が [TBD] ms 未満（先行的反応）または [TBD] ms を超える（極端な遅延反応）試行
- 誤反応率が50%を超えるセッション（課題の理解不十分が疑われる）
- 5問以上の無回答が含まれるセッション

---

## 4. 引用文献


##### Banks et al. (2018)
Banks, W. A., Owen, J. B., & Erickson, M. A. (2018). Insulin in the brain: There and back again. *Pharmacological Reviews*, *70*(3), 694–718. https://doi.org/10.1124/pr.118.015909


##### Brose et al. (2012)
Brose, A., Schmiedek, F., Lövdén, M., & Lindenberger, U. (2012). Daily variability in working memory is coupled with negative affect: The role of attention and motivation. *Emotion*, *12*(3), 605–617. https://doi.org/10.1037/a0024436


##### Campbell et al. (2020)
Campbell, L. M., Paolillo, E. W., Heaton, A., Tang, B., Depp, C. A., Granholm, E., & Moore, R. C. (2020). Daily activities related to mobile cognitive performance in middle-aged and older adults: An ecological momentary cognitive assessment study. *JMIR mHealth and uHealth*, *8*(9), e19579. https://doi.org/10.2196/19579


##### Chaytor et al. (2023)
Chaytor, N. S., Gerstner, E. C., Fonseca, L. M., Germine, L. T., Hawks, Z. W., Kudva, Y. C., Pratley, R., Rickels, M. R., Rizvi, S. R., Singh, S., Weinstock, R. S., & Sliwinski, M. J. (2023). Glycemic variability and fluctuations in cognitive status in adults with Type 1 Diabetes (GluCog): Observational study using ecological momentary assessment of cognition. *JMIR mHealth and uHealth*, *8*, e39750. https://doi.org/10.2196/39750


##### Falleti et al. (2006)
Falleti, M. G., Maruff, P., Collie, A., & Darby, D. G. (2006). Practice effects associated with the repeated assessment of cognitive function using the CogState battery at 10-minute, one week and one month test-retest intervals. *Journal of Clinical and Experimental Neuropsychology*, *28*(7), 1095–1112. https://doi.org/10.1080/13803390500205718


##### Formánek et al. (2020)
Formánek, T., Csajbók, Z., Wolfová, K., et al. (2020). Trajectories of depressive symptoms and associated patterns of cognitive decline. *Scientific Reports*, *10*, 20888. https://doi.org/10.1038/s41598-020-77866-6


##### Hawks et al. (2024)
Hawks, Z. W., Beck, E. D., Jung, L., Fonseca, L. M., Sliwinski, M. J., Weinstock, R. S., Grinspoon, E., Xu, I., Strong, R. W., Singh, S., Van Dongen, H. P. A., Frumkin, M. R., Bulger, J., Cleveland, M. J., Janess, K., Kudva, Y. C., Pratley, R., Rickels, M. R., Rizvi, S. R., Chaytor, N. S., & Germine, L. T. (2024). Dynamic associations between glucose and ecological momentary cognition in Type 1 Diabetes. *npj Digital Medicine*, *7*, 59. https://doi.org/10.1038/s41746-024-01036-5


##### Ingwersen et al. (2012)
Ingwersen, J., Defeyter, M. A., Kennedy, D. O., Wesnes, K. A., & Scholey, A. B. (2012). Effects on cognitive performance of modulating the postprandial blood glucose profile at breakfast. *European Journal of Clinical Nutrition*, *66*(9), 1053–1058. https://doi.org/10.1038/ejcn.2012.80


##### Kim et al. (2022)
Kim, H. J., Kim, S. M., Lee, G., et al. (2022). Association between visit-to-visit fasting glycemic variability and depression: A retrospective cohort study in a representative Korean population without diabetes. *Scientific Reports*, *12*, 18692. https://doi.org/10.1038/s41598-022-22302-0


##### Kirchner (1958)
Kirchner, W. K. (1958). Age differences in short-term retention of rapidly changing information. *Journal of Experimental Psychology*, *55*(4), 352–358. https://doi.org/10.1037/h0043688


##### Kwon et al. (2023)
Kwon, M., Lee, M., Kim, E. H., et al. (2023). Risk of depression and anxiety disorders according to long-term glycemic variability. *Journal of Affective Disorders*, *343*, 50–58. https://doi.org/10.1016/j.jad.2023.09.017


##### Lezak et al. (2004)
Lezak, M. D., Howieson, D. B., & Loring, D. W. (2004). *Neuropsychological assessment* (4th ed.). Oxford University Press.


##### Nilsson et al. (2012)
Nilsson, A., Radeborg, K., & Björck, I. (2012). Effects of differences in postprandial glycaemia on cognitive functions in healthy middle-aged subjects. *European Journal of Clinical Nutrition*, *66*(9), 1056–1062. https://doi.org/10.1038/ejcn.2007.173


##### Noetel et al. (2024)
Noetel, M., Sanders, T., Gallardo-Gómez, D., Taylor, P., Del Pozo Cruz, B., Van Den Hoek, D., Smith, J. J., Mahoney, J., Spathis, D., Moresi, M., Pagano, R., Charlton, K., Lyons-Wall, P., Abbott, G., Vasconcellos, R., Parker, P., & Lonsdale, C. (2024). Effect of exercise for depression: Systematic review and network meta-analysis of randomised controlled trials. *BMJ*, *384*, e075847. https://doi.org/10.1136/bmj-2023-075847


##### Pearce et al. (2022)
Pearce, M., Garcia, L., Abbas, A., Strain, T., Schuch, F. B., Golubic, R., Kelly, P., Khan, S., Utukuri, M., Laird, Y., Mok, A., Smith, A., Tainio, M., Brage, S., & Woodcock, J. (2022). Association between physical activity and risk of depression: A systematic review and meta-analysis. *JAMA Psychiatry*, *79*(6), 550–559. https://doi.org/10.1001/jamapsychiatry.2022.0609


##### Radloff (1977)
Radloff, L. S. (1977). The CES-D scale: A self-report depression scale for research in the general population. *Applied Psychological Measurement*, *1*(3), 385–401. https://doi.org/10.1177/014662167700100306


##### Schaich et al. (2024)
Schaich, C. L., et al. (2024). 【確認中：詳細書誌情報を補完してください】


##### Schmitter-Edgecombe et al. (2024)
Schmitter-Edgecombe, M., Luna, C., Beech, B., Dai, S., & Cook, D. J. (2024). Capturing cognitive capacity in the everyday environment across a continuum of cognitive decline using a smartwatch n-back task and ecological momentary assessment. *Neuropsychology*, *39*(1), 28–43. https://doi.org/10.1037/neu0000984


##### 島ら（1985）
島 悟・鹿野 友章・北村 俊則・浅井 昌弘 (1985). 新しい抑うつ性自己評価尺度について. *精神医学*, *27*(6), 717–723.


##### Sliwinski et al. (2018)
Sliwinski, M. J., Mogle, J. A., Hyun, J., Munoz, E., Smyth, J. M., & Lipton, R. B. (2018). Reliability and validity of ambulatory cognitive assessments. *Assessment*, *25*(1), 14–30. https://doi.org/10.1177/1073191116643164


##### Takahashi et al. (2018)
Takahashi, M., Ozaki, M., Kang, M.-I., Sasaki, H., Fukazawa, M., Iwakami, T., Lim, P. J., Kim, H.-K., Aoyama, S., & Shibata, S. (2018). Effects of meal timing on postprandial glucose metabolism and blood metabolites in healthy adults. *Nutrients*, *10*(11), 1763. https://doi.org/10.3390/nu10111763


##### Yin et al. (2024)
Yin, J., John, A., & Cadar, D. (2024). Bidirectional associations of depressive symptoms and cognitive function over time. *JAMA Network Open*, *7*(6), e2416305. https://doi.org/10.1001/jamanetworkopen.2024.16305


##### Yu et al. (2020)
Yu, Z. B., Zhu, Y., Li, D., Wu, M. Y., Tang, M. L., Wang, J. B., & Chen, K. (2020). Association between visit-to-visit variability of HbA1c and cognitive decline: A pooled analysis of two prospective population-based cohorts. *Diabetologia*, *63*(1), 85–94. https://doi.org/10.1007/s00125-019-04986-8


##### Zlatar et al. (2022)
Zlatar, Z. Z., Campbell, L. M., Tang, B., Gabin, S., Heaton, A., Higgins, M., Villalobos, E. I., Moore, D. J., & Moore, R. C. (2022). Daily level association of physical activity and performance on ecological momentary cognitive tests in free-living environments: A mobile health observational study. *JMIR mHealth and uHealth*, *10*(1), e33747. https://doi.org/10.2196/33747

---

## 付記：今後確定すべき事項（[TBD]の内訳）

| 項目 | 検討状況 |
|------|---------|
| GradCPT：練習試行数 | 先行研究レビュー後に決定 |
| DSM：試行数・制限時間 | 同上 |
| DSM：数字-シンボル対応表の種類 | 同上 |
| 2-back：使用文字セット | 同上 |
| 2-back：刺激提示時間・ISI | 同上 |
| 2-back：本番試行数 | 同上 |
| 反応時間の除外基準（上下限） | 同上 |

---

*本文書はプレレジ提出用の草稿であり，OSF（Open Science Framework）への登録時に最終版として確定する予定である。*
