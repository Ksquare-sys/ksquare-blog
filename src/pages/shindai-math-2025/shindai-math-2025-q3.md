---
title: "神戸大学理系数学の過去問傾向と対策｜2025年第3問・媒介変数と微積を完全攻略"
description: "神戸大学（理系）数学2025年過去問解説。最頻出分野である「媒介変数表示の曲線と微積分」をテーマに、2025年第3問を用いて、曲線の対称性の見抜き方や絶対値を含む積分の計算ポイントを徹底解説します。"
---
<title>神戸大学理系数学の過去問傾向と対策｜2025年第3問・媒介変数と微積を完全攻略</title>
<link rel="icon" type="image/png" href="/favicon.png" />
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.css">

# 神戸大学（理系）数学で絶対に差がつく「媒介変数と微積」の融合問題

神戸大学の理系数学において、合格ラインを突破するために避けて通れないのが「微分積分」と「媒介変数表示の曲線」の融合問題です。

これらの問題は、一見複雑そうに見えても、曲線の対称性を正しく数式から見抜き、計算をいかに効率化できるかで勝負が決まります。

本日は、2025年度の第3問を題材に、媒介変数表示の曲線を解きほぐす「発想のポイント」と「積分の注意点」を徹底解説します。

---

## 📝 今日の過去問（2025年度 第3問）

まずは、今回のターゲットとなる問題を確認しましょう。

![2025年第3問 問題画像](/images/kouberikei_2025_3.png)

---

## 🔗 2025年度・他の大問の解説はこちら

* [大問1（微分）](./kouberikei-2025-q1)
* [大問2（数列）](./kouberikei-2025-q2)
* **大問3（積分 ※本記事）**
* [大問4（ベクトル）](./kouberikei-2025-q4)
* [大問5（微分）](./kouberikei-2025-q5)

---
## 📊 過去問研究データ：神戸大の出題ヒートマップ

なぜ、このテーマを完璧にする必要があるのか。その理由は、こちらの過去問分析データにあります。

![神戸大数学ヒートマップ](/images/kouberikei.png)

神戸大の理系数学において、微分積分（媒介変数を含む）の問題は、出題率ナンバーワンの「超・最頻出分野」です。特に、曲線が囲む面積を求める問題は、形を変えて何度も出題されています。

ここをスムーズに解き切れるかどうかが、神戸大合格への大きな鍵となります。

---

## 💡 発想のポイント：神戸大の問題は対称性に注意せよ

神戸大の媒介変数問題を攻略するためのポイントは以下の3つです。

> **⏰ 発想のポイント①：「媒介変数は対称性に注意。見抜き方は2パターン」**
>
> 媒介変数表示された曲線の概形を考える際、闇雲に増減表を作る前に、まずは対称性を調べることが鉄則です。見抜き方は大きく分けて以下の2パターンがあります。
> ① $\theta$ に $-\theta$ や $2\pi - \theta$ などを代入して、$x$ や $y$ の符号・形がどう変わるかを確認する。
> ② 媒介変数 $\theta$ を消去して、直交座標表示（$x$ と $y$ の関係式）を導いてみる。
> 本問では、$\theta$ を $2\pi - \theta$ に置き換えることで、$y$ 軸対称であることが一瞬で見抜けます。

> **✨ 発想のポイント②：「絶対値を見たら外す」**
>
> 式の中に $|\sin \theta|$ という絶対値が含まれています。数学の基本に忠実に、中身が正になるか負になるかで必ず場合分けを行いましょう。今回は $0 \leqq \theta \leqq 2\pi$ なので、$0 \leqq \theta \leqq \pi$（$\sin \theta \geqq 0$）と $\pi \leqq \theta \leqq 2\pi$（$\sin \theta \leqq 0$）で切り離して考えます。

> **❄️ 発想のポイント③：「対称性を活かして積分区間を簡略化する」**
>
> (2)の面積計算では、(1)で判明した曲線の対称性（$y$ 軸対称）を最大限に利用します。グラフ全体で積分を計算するのではなく、第一象限（または $x \geqq 0$ の範囲）の面積を求めてからそれを「2倍」にすることで、計算ミスを大幅に減らすことができます。

## ✍️ 模範解答

### (1) 曲線 $C$ の対称性および $C$ と $y$ 軸との共有点の座標を求めよ

**[対称性について]**
曲線 $C$ の方程式は
$$ \begin{cases} x = a \sin \theta \cos \theta & \cdots ① \\ y = |\sin \theta| \sin \theta + \sin \theta & \cdots ② \end{cases} $$
である。
①より、$x = \frac{1}{2} a \sin 2\theta$ であるため、$x$ の周期は $\pi$ である。
また、②において、$-\pi \leqq \theta \leqq \pi$ の範囲（$\theta = t$ とおく）で考えると、
$\theta = t$ のとき、$y = |\sin t|\sin t + \sin t$
$\theta = -t$ のとき、$y = |\sin(-t)|\sin(-t) + \sin(-t) = |-\sin t|(-\sin t) - \sin t = -|\sin t|\sin t - \sin t$
となり、$y(-t) = -y(t)$ である。すなわち、$\theta$ の範囲を $2\pi$ 周期（例えば $-\pi$ から $\pi$）で考えると、曲線 $C$ は原点対称であるが、本問の範囲は $0 \leqq \theta \leqq 2\pi$ であるため、注意が必要である。

$\theta$ を $2\pi - \theta$ （ただし $0 \leqq \theta \leqq \pi$）に置き換えると、
$$ \begin{aligned} x(2\pi-\theta) &= a \sin(2\pi-\theta) \cos(2\pi-\theta) \\ &= a(-\sin\theta)\cos\theta \\ &= -a\sin\theta\cos\theta \\ &= -x(\theta) \\ y(2\pi-\theta) &= |\sin(2\pi-\theta)| \sin(2\pi-\theta) + \sin(2\pi-\theta) \\ &= |-\sin\theta| (-\sin\theta) + (-\sin\theta) \\ &= |\sin\theta| (-\sin\theta) - \sin\theta \\ &= -(|\sin\theta|\sin\theta + \sin\theta) \\ &= -y(\theta) \end{aligned} $$
となる。
すなわち、曲線 $C$ 上の点 $(x(\theta), y(\theta))$ に対して、点 $(-x(\theta), -y(\theta))$ も曲線 $C$ 上に存在する。
よって、曲線 $C$ は **原点対称** である。

**[y軸との共有点について]**
共有点の $x$ 座標は $0$ であるため、
$$ \begin{aligned} a \sin \theta \cos \theta &= 0 \\ \frac{1}{2} a \sin 2\theta &= 0 \end{aligned} $$
$a > 0$ かつ $0 \leqq \theta \leqq 2\pi$ より、$\sin 2\theta = 0$ となる $2\theta$ の値は、
$$ 2\theta = 0, \pi, 2\pi, 3\pi, 4\pi $$
$$ \therefore \theta = 0, \frac{\pi}{2}, \pi, \frac{3}{2}\pi, 2\pi $$
である。それぞれの $\theta$ の値に対する $y$ の値を求める。

[i] $\theta = 0, \pi, 2\pi$ のとき
$$ y = |\sin \theta|\sin \theta + \sin \theta = 0 \cdot 0 + 0 = 0 $$
[ii] $\theta = \frac{\pi}{2}$ のとき
$$ y = |\sin \frac{\pi}{2}|\sin \frac{\pi}{2} + \sin \frac{\pi}{2} = 1 \cdot 1 + 1 = 2 $$
[iii] $\theta = \frac{3}{2}\pi$ のとき
$$ y = |\sin \frac{3}{2}\pi|\sin \frac{3}{2}\pi + \sin \frac{3}{2}\pi = |-1| \cdot (-1) + (-1) = -2 $$

以上、[i]〜[iii]より、求める共有点の座標は **$(0, 0), (0, 2), (0, -2)$** である。

---

### (2) 曲線 $C$ の概形をかけ

(1)より曲線 $C$ は原点対称であるため、$0 \leqq \theta \leqq \pi$ の範囲における概形を調べ、それを原点に関して対称移動させればよい。
$0 \leqq \theta \leqq \pi$ のとき $\sin \theta \geqq 0$ であるため、$y$ は
$$ y = (\sin \theta)\sin \theta + \sin \theta = \sin^2 \theta + \sin \theta $$
である。
また、$x = \frac{1}{2} a \sin 2\theta$ である。
これらを $\theta$ で微分すると、
$$ \frac{dx}{d\theta} = a \cos 2\theta $$
$$ \frac{dy}{d\theta} = 2\sin\theta\cos\theta + \cos\theta = \cos\theta(2\sin\theta+1) $$
$0 \leqq \theta \leqq \pi$ の範囲において、$\frac{dx}{d\theta} = 0$ となるのは $\theta = \frac{\pi}{4}, \frac{3}{4}\pi$、$\frac{dy}{d\theta} = 0$ となるのは $\theta = \frac{\pi}{2}$ である（$2\sin\theta+1 > 0$ である）。
よって、増減表は以下のようになる。

| $\theta$ | $0$ | $\cdots$ | $\frac{\pi}{4}$ | $\cdots$ | $\frac{\pi}{2}$ | $\cdots$ | $\frac{3}{4}\pi$ | $\cdots$ | $\pi$ |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| $\frac{dx}{d\theta}$ | $+$ | $+$ | $0$ | $-$ | $-$ | $-$ | $0$ | $+$ | $+$ |
| $x$ | $0$ | $\rightarrow$ | $\frac{a}{2}$ | $\leftarrow$ | $0$ | $\leftarrow$ | $-\frac{a}{2}$ | $\rightarrow$ | $0$ |
| $\frac{dy}{d\theta}$ | $+$ | $+$ | $+$ | $+$ | $0$ | $-$ | $-$ | $-$ | $-$ |
| $y$ | $0$ | $\uparrow$ | $\frac{1+\sqrt{2}}{2}$ | $\uparrow$ | $2$ | $\downarrow$ | $\frac{1+\sqrt{2}}{2}$ | $\downarrow$ | $0$ |

※表内の $y$ 軸の値は以下の通り。
$\theta = \frac{\pi}{4}, \frac{3}{4}\pi \Rightarrow y = (\frac{\sqrt{2}}{2})^2 + \frac{\sqrt{2}}{2} = \frac{1}{2} + \frac{\sqrt{2}}{2} = \frac{1+\sqrt{2}}{2}$
$\theta = \frac{\pi}{2} \Rightarrow y = 1^2 + 1 = 2$

この増減および(1)の原点対称性より、曲線 $C$ の概形は次図の通りである。

![図1：曲線 $C$ の概形](/images/kouberikei_3_1.png)

また、グラフは $\frac{\pi}{2} < \theta < \frac{3}{2}\pi$ で $x < 0$ となるので、$y$ 軸に関する対称性も見抜くことができる。

### (3) 曲線 $C$ で囲まれた部分の面積 $S$ を求めよ

(1), (2)で確認した曲線の対称性より、曲線 $C$ は $y$ 軸に関しても対称（かつ原点対称、すなわち $x$ 軸に関しても対称）なハート型の形状をしている。
したがって、求める全体の面積 $S$ は、第1象限（$x \geqq 0, y \geqq 0$）の面積を4倍、あるいは $x \geqq 0$ の範囲の面積を2倍にすることで計算を簡略化できる。

ここでは、曲線 $C$ の $y$ 軸対称性を考慮し、$x \ge 0$ （すなわち $0 \leqq \theta \leqq \frac{\pi}{2}$ および $\frac{3}{2}\pi \leqq \theta \leqq 2\pi$）の範囲において、上側の曲線を $y_1$、下側の曲線を $y_2$ とおく。

$$ S = 2 \left( \int_{0}^{1} y_1 dx - \int_{0}^{1} y_2 dx \right) $$

ここで、$x = \sin \theta$ より、$\frac{dx}{d\theta} = \cos \theta$ である。
積分区間 $x: 0 \to 1$ に対応する $\theta$ の範囲は以下のようになる。
* $y_1$（上側・大半が $0 \leqq \theta \leqq \frac{\pi}{2}$）：$\theta$ は $0 \to \frac{\pi}{2}$
* $y_2$（下側・大半が $\frac{\pi}{2} \leqq \theta \leqq \pi$）：$\theta$ は $\pi \to \frac{\pi}{2}$

これらを置換積分により $\theta$ の積分に直すと、
$$ \begin{aligned} S &= 2 \left( \int_{0}^{\frac{\pi}{2}} y_1 \cdot \cos \theta d\theta - \int_{\pi}^{\frac{\pi}{2}} y_2 \cdot \cos \theta d\theta \right) \\ &= 2 \left( \int_{0}^{\frac{\pi}{2}} (\cos \theta + \sin \theta)\cos \theta d\theta + \int_{\frac{\pi}{2}}^{\pi} (\cos \theta + \sin \theta)\cos \theta d\theta \right) \\ &= 2 \int_{0}^{\pi} (\cos^2 \theta + \sin \theta \cos \theta) d\theta \end{aligned} $$

ここで、2倍角の公式および半角の公式
$$ \cos^2 \theta = \frac{1 + \cos 2\theta}{2}, \quad \sin \theta \cos \theta = \frac{\sin 2\theta}{2} $$
を利用して被積分関数を変形する。

$$ \begin{aligned} S &= 2 \int_{0}^{\pi} \left( \frac{1 + \cos 2\theta + \sin 2\theta}{2} \right) d\theta \\ &= \int_{0}^{\pi} (1 + \cos 2\theta + \sin 2\theta) d\theta \\ &= \left[ \theta + \frac{1}{2}\sin 2\theta - \frac{1}{2}\cos 2\theta \right]_{0}^{\pi} \\ &= \left( \pi + 0 - \frac{1}{2} \right) - \left( 0 + 0 - \frac{1}{2} \right) \\ &= \pi \end{aligned} $$

よって、求める面積は **$S = \pi$** となる。

---

<style>
  .ksq-cta { background:#fbf8f3; margin-top:40px; color:#16202e; font-family:'Noto Sans JP','Hiragino Kaku Gothic ProN',sans-serif; container-type:inline-size; }
  .ksq-cta * { box-sizing:border-box; }
  .ksq-cta-inner { padding:72px 64px; }
  .ksq-eyebrow { display:flex; align-items:center; justify-content:space-between; margin-bottom:48px; flex-wrap:wrap; gap:12px; }
  .ksq-wordmark { font-family:'Cormorant Garamond','Noto Serif JP',serif; font-size:22px; color:#0b2240; font-weight:500; letter-spacing:-0.01em; }
  .ksq-grid { display:grid; grid-template-columns:240px 1fr; gap:48px; align-items:start; }
  .ksq-num-wrap { position:relative; }
  .ksq-num { font-family:'Cormorant Garamond','Noto Serif JP',serif; font-size:200px; line-height:0.85; color:#0b2240; font-weight:500; letter-spacing:-0.05em; }
  .ksq-num-label { position:absolute; top:18px; right:-2px; font-family:'Shippori Mincho','Noto Serif JP',serif; font-size:16px; color:#0b2240; writing-mode:vertical-rl; letter-spacing:0.3em; }
  .ksq-num-rule { margin-top:12px; padding-top:16px; border-top:1px solid #0b2240; font-size:11px; color:#0b2240; letter-spacing:0.16em; font-weight:600; }
  .ksq-num-note { margin-top:16px; font-size:12px; line-height:1.8; color:#3a4452; }
  .ksq-tag { font-family:'Shippori Mincho','Noto Serif JP',serif; font-size:clamp(36px, 6vw, 56px); letter-spacing:0.1em; color:#9b2a2a; font-weight:800; margin-top:-80px; margin-bottom:20px; line-height:1.2; }
  .ksq-h2 { font-family:'Shippori Mincho','Noto Serif JP',serif; font-size:clamp(28px,4vw,40px); line-height:1.4; font-weight:500; color:#16202e; margin:0 0 28px; letter-spacing:0.01em; }
  .ksq-body { margin:0 0 36px; font-size:14.5px; line-height:2; color:#2a3340; max-width:540px; }
  .ksq-btn { display:flex; align-items:stretch; width:100%; text-decoration:none; color:#fff; box-shadow:0 18px 36px rgba(11,34,64,0.18); transition:transform .15s ease, box-shadow .15s ease; }
  .ksq-btn:hover { transform:translateY(-2px); box-shadow:0 22px 44px rgba(11,34,64,0.25); }
  .ksq-btn-slab { background:#06C755; padding:20px 24px; display:flex; flex-direction:column; align-items:center; justify-content:center; flex:0 0 auto; min-width:104px; }
  .ksq-btn-slab svg { width:32px; height:32px; margin-bottom:6px; }
  .ksq-btn-slab .lbl { font-size:13px; font-weight:800; letter-spacing:0.14em; color:#fff; }
  .ksq-btn-body { flex:1; min-width:0; background:#0b2240; padding:20px 28px; display:flex; align-items:center; justify-content:space-between; gap:16px; }
  .ksq-btn-text { display:flex; flex-direction:column; gap:6px; min-width:0; }
  .ksq-btn-title { font-size:clamp(18px,2.4vw,24px); font-weight:800; letter-spacing:0.04em; line-height:1.3; white-space:nowrap; }
  .ksq-btn-sub { font-size:12.5px; color:rgba(255,255,255,0.72); letter-spacing:0.04em; margin-top:2px; line-height:1.5; }
  .ksq-btn-arrow { display:inline-flex; align-items:center; justify-content:center; width:48px; height:48px; border-radius:50%; border:1px solid rgba(255,255,255,0.45); font-size:22px; flex-shrink:0; }
  .ksq-trust { display:flex; align-items:center; gap:14px 22px; margin-top:22px; font-size:11.5px; color:#5a6473; letter-spacing:0.06em; flex-wrap:wrap; }
  .ksq-trust .sep { width:1px; height:12px; background:#d8d2c4; }
  @container (max-width: 980px) {
    .ksq-cta-inner { padding:48px 28px; }
    .ksq-grid { grid-template-columns:1fr; gap:24px; }
    .ksq-num-wrap { display:flex; align-items:baseline; gap:14px; border-bottom:1px solid #d8d2c4; padding-bottom:20px; }
    .ksq-num { font-size:64px; line-height:1; letter-spacing:-0.03em; }
    .ksq-num-label { position:static; writing-mode:horizontal-tb; font-size:18px; letter-spacing:0.18em; font-weight:500; }
    .ksq-num-rule, .ksq-num-note { display:none; }
    .ksq-tag { margin-top: 24px; }
    .ksq-btn-title { white-space:normal; }
    .ksq-trust .sep { display:none; }
  }
  @container (max-width: 600px) {
    .ksq-cta-inner { padding:36px 20px; }
    .ksq-eyebrow { margin-bottom:28px; gap:8px; }
    .ksq-wordmark { font-size:19px; }
    .ksq-num { font-size:56px; }
    .ksq-num-label { font-size:15px; letter-spacing:0.14em; }
    .ksq-tag { font-size:28px; letter-spacing:0.05em; margin-top:20px; margin-bottom:12px; }
    .ksq-h2 { font-size:24px; line-height:1.5; margin:0 0 22px; }
    .ksq-body { font-size:13.5px; line-height:1.9; margin:0 0 28px; }
    .ksq-btn { flex-direction:column; }
    .ksq-btn-slab { flex-direction:row; gap:10px; padding:14px 20px; min-width:0; width:100%; justify-content:center; }
    .ksq-btn-slab svg { width:22px; height:22px; margin-bottom:0; }
    .ksq-btn-body { padding:22px 20px; }
    .ksq-btn-title { font-size:19px; letter-spacing:0.02em; }
    .ksq-btn-sub { font-size:12px; }
    .ksq-btn-arrow { width:40px; height:40px; font-size:18px; }
    .ksq-trust { font-size:11px; gap:8px; margin-top:18px; }
  }
</style>

<div class="ksq-cta">
<div class="ksq-cta-inner">
  <div class="ksq-eyebrow">
    <div class="ksq-wordmark">Ksquare<sup style="font-size:0.4em; vertical-align:super;">K²</sup> ／ 志望校特化塾</div>
  </div>
  <div class="ksq-grid">
    <div class="ksq-num-wrap">
      <div class="ksq-num">10</div>
      <div class="ksq-num-label">年分の研究</div>
      <div class="ksq-num-rule">YEARS OF PAST-EXAM ANALYSIS</div>
      <p class="ksq-num-note">出題分野・難度・解答時間配分まで、志望校ごとに独自データベース化。</p>
    </div>
    <div>
      <div class="ksq-tag">志望校特化の戦略で、逆転合格を。</div>
      <h2 class="ksq-h2">「過去問で点が取れる」<br>その圧倒的な実感を、あなたへ。</h2>
      <p class="ksq-body">学校や集団塾ではしてくれない、志望大学の過去問<strong style="color:#0b2240;">10年単位の研究</strong>に基づくオーダーメイドのカリキュラム。最難関大合格講師が、あなたの志望校の過去問を頻出分野の列挙にとどまらない、出題パターンまでの研究。Ksquareは、合格点を最短で取りに行く志望校専門塾です。</p>
      <a class="ksq-btn" href="https://lin.ee/X5acA6L">
        <div class="ksq-btn-slab">
          <svg viewBox="0 0 32 32" fill="none" aria-hidden="true"><path d="M16 4C8.82 4 3 8.7 3 14.5c0 3.7 2.4 6.95 6 8.83V29l5.4-3.6c.52.04 1.06.07 1.6.07 7.18 0 13-4.7 13-10.47S23.18 4 16 4z" fill="#fff"></path></svg>
          <span class="lbl">LINE</span>
        </div>
        <div class="ksq-btn-body">
          <div class="ksq-btn-text">
            <span class="ksq-btn-title">公式LINEでコースを見る</span>
            <span class="ksq-btn-sub">志望校別のカリキュラム・料金・合格事例をその場でチェック</span>
          </div>
          <span class="ksq-btn-arrow">→</span>
        </div>
      </a>
      <div class="ksq-trust">
        <span>○ 友だち追加だけ・しつこい営業なし</span>
        <span class="sep"></span>
        <span>○ 無料の戦略診断（面談）もLINEから</span>
        <span class="sep"></span>
        <span>○ 毎月の受入人数に上限あり</span>
      </div>
    </div>
  </div>
</div>
</div>