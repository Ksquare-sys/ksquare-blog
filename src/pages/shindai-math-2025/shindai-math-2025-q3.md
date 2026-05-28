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

### (1) 曲線 $C$ の概形をかけ

いま、$f(\theta) = \sin \theta, \; g(\theta) = \cos \theta + |\sin \theta|$ とすると、絶対値記号の外れ方から $g(\theta)$ は以下のように場合分けされる。

$$
g(\theta) = \begin{cases} \cos \theta + \sin \theta & (0 \leqq \theta \leqq \pi) \\ \cos \theta - \sin \theta & (\pi \leqq \theta \leqq 2\pi) \end{cases}
$$

ここで、$\theta$ の範囲で場合分けをして増減を調べる。

**[1] $0 \leqq \theta \leqq \pi$ のとき**
このとき、$f(\theta) = \sin \theta, \; g(\theta) = \cos \theta + \sin \theta$ より、各関数を $\theta$ で微分すると、
$$ f'(\theta) = \cos \theta, \quad g'(\theta) = -\sin \theta + \cos \theta $$
となる。
三角関数の合成より、$-\sin \theta + \cos \theta = \sqrt{2}\cos\left(\theta + \frac{\pi}{4}\right)$ であるから、
$0 \leqq \theta \leqq \pi$ の範囲で $f'(\theta) = 0$ となるのは $\theta = \frac{\pi}{2}$ のとき。
$g'(\theta) = 0$ となるのは $\theta = \frac{\pi}{4}$ のときである。
よって、この区間における増減表は次表のようになる。
$$
\begin{array}{|c|c|c|c|c|c|c|c|}
\hline
\theta & 0 & \cdots & \frac{\pi}{4} & \cdots & \frac{\pi}{2} & \cdots & \pi \\ \hline
f'(\theta) & & + & + & + & 0 & - & \\ \hline
g'(\theta) & & + & 0 & - & - & - & \\ \hline
f(\theta) \ (x) & 0 & \nearrow & \frac{\sqrt{2}}{2} & \nearrow & 1 & \searrow & 0 \\ \hline
g(\theta) \ (y) & 1 & \nearrow & \sqrt{2} & \searrow & 1 & \searrow & -1 \\ \hline
\end{array}
$$
ここで、$g(\theta) = 0$ となるのは、$g(\theta) = \sqrt{2}\cos\left(\theta - \frac{\pi}{4}\right)$ に注意すると、$\theta = \frac{3}{4}\pi$ のときであり、このとき $f\left(\frac{3}{4}\pi\right) = \frac{\sqrt{2}}{2}$ となる。
よって、$x$ 切片は $\left(\frac{\sqrt{2}}{2}, 0\right)$ となり、$y$ 切片は $(0, 1), (0, -1)$ となる。

**[2] $\pi \leqq \theta \leqq 2\pi$ のとき**
このとき、$f(\theta) = \sin \theta, \; g(\theta) = \cos \theta - \sin \theta$ となる。
ここで、$\pi \leqq \theta \leqq 2\pi$ より、$0 \leqq 2\pi - \theta \leqq \pi$ であることに注意して、$\theta$ を $2\pi - \theta$ に置き換えて対称性を調べると、

$$
\begin{aligned}
f(2\pi - \theta) &= \sin(2\pi - \theta) \\
&= -\sin \theta \\
&= -f(\theta)
\end{aligned}
$$
$$
\begin{aligned}
g(2\pi - \theta) &= \cos(2\pi - \theta) + |\sin(2\pi - \theta)| \\
&= \cos \theta + |-\sin \theta| \\
&= \cos \theta + |\sin \theta| \\
&= g(\theta)
\end{aligned}
$$

であるから、このときのグラフは [1] で求めた $0 \leqq \theta \leqq \pi$ のときの曲線を $y$ 軸に対して折り返したもの（$y$ 軸対称）となる。

以上、[1], [2] より、$x = \sin \theta, \; y = \cos \theta + |\sin \theta|$ で表される曲線 $C$ の概形は、次図のようなハート型になる。

![図1：曲線 $C$ の概形](/images/kouberikei_3_1.png)

---

### (2) 曲線 $C$ で囲まれた部分の面積を求めよ

いま、曲線 $C$ に囲まれた部分の面積を $S$ とし、また $0 \leqq \theta \leqq \frac{\pi}{2}, \; \frac{\pi}{2} \leqq \theta \leqq \pi$ の各区間における $y$ をそれぞれ $y_1, y_2$ とする。
曲線 $C$ の $y$ 軸対称性を考慮すると、求める面積 $S$ は $x \geqq 0$ 側の面積を2倍すればよいので、

$$ S = 2\left( \int_{0}^{1} y_1 dx - \int_{0}^{1} y_2 dx \right) $$

となる。ここで、$x = \sin \theta$ より、$\frac{dx}{d\theta} = \cos \theta$ であるから、置換積分を行うと、

$$
\begin{aligned}
S &= 2\left( \int_{0}^{1} y_1 dx - \int_{0}^{1} y_2 dx \right) \\
&= 2\left( \int_{0}^{\frac{\pi}{2}} (\cos \theta + \sin \theta)\cos \theta d\theta - \int_{\pi}^{\frac{\pi}{2}} (\cos \theta + \sin \theta)\cos \theta d\theta \right) \\
&= 2\left( \int_{0}^{\frac{\pi}{2}} (\cos^2 \theta + \sin \theta \cos \theta) d\theta + \int_{\frac{\pi}{2}}^{\pi} (\cos^2 \theta + \sin \theta \cos \theta) d\theta \right) \\
&= 2\int_{0}^{\pi} (\cos^2 \theta + \sin \theta \cos \theta) d\theta \\
&= 2\int_{0}^{\pi} \left( \frac{1 + \cos 2\theta + \sin 2\theta}{2} \right) d\theta \\
&= \left[ \theta + \frac{1}{2}\sin 2\theta - \frac{1}{2}\cos 2\theta \right]_{0}^{\pi} \\
&= \pi
\end{aligned}
$$

となる。

**（答） $\pi$**

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