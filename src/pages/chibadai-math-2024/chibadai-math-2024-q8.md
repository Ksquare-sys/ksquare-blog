---
title: "千葉大学理系数学の過去問傾向と対策｜2024年第8問・図形と極限を完全攻略"
description: "千葉大学（理系）数学の過去問データ。最頻出分野である「微積分・極限」と「図形」の融合問題をテーマに、2024年第8問を用いて、図形的性質の数式化と場合分けのポイントを徹底解説します。"
---
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.css">

# 千葉大学（理系）数学で絶対に差がつく「図形と極限」の融合問題

千葉大学の理系数学において、合格ラインを突破するために避けて通れないのが「微分積分・極限」と「図形」の融合問題です。

これらの問題は、一見複雑そうに見えても、図形的な性質を正しく数式へ落とし込めるかで勝負が決まります。

本日は、2024年度の第8問を題材に、図形問題を解きほぐす「発想のポイント」と「場合分けの注意点」を徹底解説します。

---

## 📝 今日の過去問（2024年度 第8問）

まずは、今回のターゲットとなる問題を確認しましょう。

![2024年第8問 問題画像](/images/chibadairikei_2024_8.png)

---

## 🔗 2024年度・他の大問の解説はこちら

* [大問4（小問集合）](./chibadairikei-2024-q4)
* [大問5（確率・極限）](./chibadairikei-2024-q5)
* [大問6（積分）](./chibadairikei-2024-q6)
* [大問7（極限）](./chibadairikei-2024-q7)
* **大問8（平面図形・極限 ※本記事）**

---
## 📊 過去問研究データ：千葉大の出題ヒートマップ

なぜ、このテーマを完璧にする必要があるのか。その理由は、こちらの過去問分析データにあります。

![千葉大数学ヒートマップ](/images/chibadairikei.png)

千葉大の理系数学において、微分積分・極限の問題は、出題率ナンバーワンの「超・最頻出分野」です。特に、図形的な状況を極限に飛ばす問題は、形を変えて何度も出題されています。

ここをスムーズに解き切れるかどうかが、千葉大合格への大きな鍵となります。

---

## 💡 発想のポイント：千葉大の問題は場合分けに注意せよ

千葉大の図形問題を攻略するためのポイントは以下の3つです。

> **⏰ 発想のポイント①：「一般的な図を書いて、θ,p,qの関係を調べる」**
>
> まずは、$0 < \theta < \pi$ の一般的な状況を表す図を書き、接する円の位置関係（中心間の距離＝半径の和、など）から、$\theta, p, q$ の関係式（余弦定理など）を導きます。

> **✨ 発想のポイント②：「場合分けを恐れない」**
>
> 問題文に条件（例えば、ある角が $90^\circ$）がある場合、その瞬間に図形的な状況が一変することがあります。一般的な関係式が使えない、あるいはもっと単純な関係が成り立つ場合があるため、状況に応じた場合分けが必要です。

> **❄️ 発想のポイント③：「極限公式の利用」**
>
> 図形的に $\theta \to +0$ としたとき、$q$ がどうなるかを考える際、得られた式が不定形になることがあります。その場合は、$\lim_{x \to 0} \frac{\sin x}{x} = 1$ や $\lim_{x \to 0} \frac{1-\cos x}{x^2} = \frac{1}{2}$ といった、典型的な極限公式が使える形に変形することを意識しましょう。
## ✍️ 模範解答

### (1) $q$ を $p$ と $\theta$ を用いて表す

円 $C, C_1, C_2, C_3$ の位置関係を考えるにあたり、$\theta$ の値によって場合分けをする。

**[1] $\theta = \pi$ のとき**
3円 $C, C_1, C_2$ の位置関係は下図の通りである。

![図1：$\theta=\pi$の場合の3円](/images/chibadairikei_8_1.png)

上図より、
$$2p + 2q = 2$$
$$\therefore q = 1-p$$
である。

**[2] $0 < \theta < \pi$ のとき**
3円 $C, C_1, C_2$ の位置関係は下図の通りである。

![図2：$0<\theta<\pi$の場合の3円](/images/chibadairikei_8_2.png)

円 $C_1, C_2$ は円 $C$ にそれぞれ内接するため、$OD = 1-p, OE = 1-q$ である。  また、円 $C_1, C_2$ は互いに外接するため、$DE = p+q$ である。<br>よって、三角形 $ODE$ について、余弦定理より、<br>
$$DE^2 = OD^2 + OE^2 - 2 \cdot OD \cdot OE \cdot \cos \theta$$  
$$\Leftrightarrow (p+q)^2 = (1-p)^2 + (1-q)^2 - 2(1-p)(1-q)\cos \theta$$  
$$\Leftrightarrow p^2 + 2pq + q^2 = (p^2 - 2p + 1) + (q^2 - 2q + 1) - 2(1-p)\cos \theta + 2(1-p)q\cos \theta$$  
$$\Leftrightarrow q\{p+1-(1-p)\cos \theta\} = 1-p-(1-p)\cos \theta$$  
$$\therefore q = \frac{(1-p)(1-\cos \theta)}{p+1-(1-p)\cos \theta} \cdots ①$$  
である。①は $\theta = \pi$ のときも成り立つため、すべての $\theta$ に対して、  
$$q = \frac{(1-p)(1-\cos \theta)}{p+1-(1-p)\cos \theta}$$  
が成り立つ。

---

### (2) $\lim_{\theta \to +0} \frac{q}{\theta^2}$ を求めよ

$$\frac{q}{\theta^2} = \frac{1-p}{p+1-(1-p)\cos \theta} \cdot \frac{1-\cos \theta}{\theta^2}$$
であり、
$$\lim_{\theta \to +0} \frac{1-\cos \theta}{\theta^2} = \lim_{\theta \to +0} \left\{ \frac{1}{1+\cos \theta} \left(\frac{\sin \theta}{\theta}\right)^2 \right\} = \frac{1}{1+1} \cdot 1^2 = \frac{1}{2}$$
であるため、<br>求める極限値は、
$$\lim_{\theta \to +0} \frac{q}{\theta^2} = \frac{1-p}{p+1-(1-p)\cdot 1} \cdot \frac{1}{2} = \frac{1-p}{2p}$$
となる。

---

### (3) $\angle DOE = \frac{\pi}{2}$ のとき、$p$ の値を求めよ

円 $C_3$ の中心を点 $F$ とし、線分 $DF$ の中点を点 $H$ とする。このとき、円 $C_1, C_3$ の半径は等しいため、点 $H$ は2円 $C_1, C_3$ の接点に等しい。

また、三角形 $EDF$ について、$ED=EF=p+q$ より、直線 $EH$ と直線 $DF$ は点 $H$ において直交する。ここで、$\theta$ が $\frac{\pi}{2}$ と一致するか否かで場合分けをする。

**[1] $\theta = \frac{\pi}{2}$ のとき**
$\angle DOE = \theta = \frac{\pi}{2} = \angle DHE$ であるため、$O=H$ であり、4円 $C, C_1, C_2, C_3$ の位置関係は次図の通りである。

![図3：$\theta=\frac{\pi}{2}$の場合の位置関係](/images/chibadairikei_8_3.png)

円 $C$ の半径は $1$ であるため、上図（$O$ と $H$ が一致し、円 $C_1$ の直径が円 $C$ の半径に等しくなる状態）より、
$$p = \frac{1}{2}$$
となる。


**[2] $\theta \neq \frac{\pi}{2}$ のとき**
$\angle DOE = \theta \neq \frac{\pi}{2} = \angle DHE$ より、$O \neq H$ であり、<br>三角形 $ODF$ について、$OD = OF = 1 - p$ より、直線 $OH$ と直線 $DF$ は点 $H$ において直交する。<br>ここで、$\theta$ と $\frac{\pi}{2}$ の大小関係により場合分けをする。

**[i] $0 < \theta < \frac{\pi}{2}$ のとき**
4円 $C, C_1, C_2, C_3$ の位置関係は次図の通りである。

![図4：$0<\theta<\frac{\pi}{2}$の場合の位置関係](/images/chibadairikei_8_4.png)

上図より、$\angle DOH = \theta$ であるため、$\sin \angle DOH = \sin \theta$ となる。

**[ii] $\frac{\pi}{2} < \theta < \pi$ のとき**
4円 $C, C_1, C_2, C_3$ の位置関係は次図の通りである。

![図5：$\frac{\pi}{2}<\theta<\pi$の場合の位置関係](/images/chibadairikei_8_5.png)

上図より、$\angle DOH = \pi - \theta$ であるため、$\sin \angle DOH = \sin(\pi - \theta) = \sin \theta$ となる。

三角形 $DOH$ について、$\angle DHO = \frac{\pi}{2}$ であるため、[i], [ii]より、
$$
\sin \angle DOH = \frac{DH}{DO} \Leftrightarrow \sin \theta = \frac{p}{1-p}
$$
が成り立つ。

以上、[1], [2]より、$0 < \theta < \pi$ のとき、$\sin \theta = \frac{p}{1-p}$、すなわち、$p = \frac{\sin \theta}{1+\sin \theta}$ が成り立つため、(1)より、
$$
\begin{aligned}
q &= \frac{\left(1 - \frac{\sin \theta}{1+\sin \theta}\right)(1-\cos \theta)}{\frac{\sin \theta}{1+\sin \theta} + 1 - \left(1 - \frac{\sin \theta}{1+\sin \theta}\right)\cos \theta} \\
&= \frac{1-\cos \theta}{1+2\sin \theta - \cos \theta} \\
&= \frac{(1-\cos \theta)(1+\cos \theta)}{(2\sin \theta+1-\cos \theta)(1+\cos \theta)} \\
&= \frac{\sin^2 \theta}{2(1+\cos \theta)\sin \theta + \sin^2 \theta} \\
&= \frac{\sin \theta}{2(1+\cos \theta) + \sin \theta}
\end{aligned}
$$
である。また、$p = \sqrt{2}-1$ のとき、
$$
\begin{aligned}
\sin \theta &= \frac{p}{1-p} \\
\Leftrightarrow \sin \theta &= \frac{\sqrt{2}-1}{1-(\sqrt{2}-1)} \\
\Leftrightarrow \sin \theta &= \frac{\sqrt{2}}{2}
\end{aligned}
$$
$$
\therefore \theta = \frac{\pi}{4}, \frac{3}{4}\pi \quad (\because 0 < \theta < \pi)
$$
となる。よって、$\theta = \frac{\pi}{4}$ のとき、
$$
q = \frac{\frac{\sqrt{2}}{2}}{2\left(1+\frac{\sqrt{2}}{2}\right) + \frac{\sqrt{2}}{2}} = \frac{1}{3+2\sqrt{2}} = 3-2\sqrt{2}
$$
となり、$\theta = \frac{3}{4}\pi$ のとき、
$$
q = \frac{\frac{\sqrt{2}}{2}}{2\left(1-\frac{\sqrt{2}}{2}\right) + \frac{\sqrt{2}}{2}} = \frac{1}{2\sqrt{2}-1} = \frac{2\sqrt{2}+1}{7}
$$
となるため、求める値は $q = 3-2\sqrt{2}, \frac{2\sqrt{2}+1}{7}$ である。

---

### (4) $\lim_{\theta \to +0} \frac{q}{p}$ を求めよ

(3)より、
$$
\frac{q}{p} = \frac{\sin \theta}{2(1+\cos \theta) + \sin \theta} \cdot \left(\frac{\sin \theta}{1+\sin \theta}\right)^{-1} = \frac{1+\sin \theta}{2(1+\cos \theta) + \sin \theta}
$$
となるため、求める極限値は、
$$
\lim_{\theta \to +0} \frac{q}{p} = \frac{1+0}{2 \cdot (1+1) + 0} = \frac{1}{4}
$$
となる。

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