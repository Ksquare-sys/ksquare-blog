---
title: "【2026年最新】横浜国立大学（理系）数学の過去問傾向と対策｜頻出の空間ベクトルを完全攻略"
description: "独自に解析した横浜国立大学（理系）数学の過去問データ。受験生が差をつけられる「空間ベクトル」の頻出パターンと、日本語を数式化する発想のポイントを実際の過去問（2024年第3問）を用いて徹底解説します。"
---
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/katex@0.16.8/dist/katex.min.css">

# 横浜国立大学（理系）数学で絶対に差がつく「空間ベクトル」の頻出パターン

横浜国立大学の理系数学において、合格ラインを突破するために避けて通れないのが「空間ベクトルの計量問題」です。

横国の空間ベクトルは、方針自体は典型的であるものの、計算量が多く、問題文の条件をいかに素早く正確に数式へ落とし込めるかで勝負が決まります。

本日は、2024年度の第3問をベースに、横国合格に必要な「翻訳力」と「解答へのアプローチ」を徹底解説します。

---

## 📝 今日の過去問（2024年度 第3問）

まずは、今回のターゲットとなる問題を確認しましょう。

![2024年第3問 問題画像](/images/yokokokurikei_2024_3.png)

---

## 🔗 2024年度・他の大問の解説はこちら

* [大問1（積分）](./yokokoku-math-2024-q1)
* [大問2（確率）](./yokokoku-math-2024-q2)
* **大問3（ベクトル ※本記事）**
* [大問4（複素数平面）](./yokokoku-math-2024-q4)
* [大問5（極限）](./yokokoku-math-2024-q5)

---
## 📊 過去問研究データ：横国の出題ヒートマップ

なぜ、この空間ベクトルを完璧にする必要があるのか。その理由は、こちらの過去問分析データにあります。

![横国数学ヒートマップ](/images/yokokokurikei.png)

横国の理系数学において、空間ベクトルは微分積分と並ぶ「超・最頻出分野」です。特に「直線と平面の交点」や「垂直条件（内積＝0）を利用した計量」は、形を変えて何度も出題されています。

ここをスムーズに解き切れるかどうかが、横国理系キャンパスへの切符を握っています。

---

## 💡 発想のポイント：日本語を「数学語（数式）」に翻訳せよ

空間ベクトルが苦手な人は、問題文の日本語をどう数式にすればいいかで迷ってしまいます。
しかし、横国を攻略するための「翻訳ルール」は以下の2つだけです。

> **⏰ 翻訳ルール①：「点 $H$ は直線 $CG$ 上にある」**
>
> 直線上の点ということは、実数 $k$ を用いて $\vec{CH} = k\vec{CG}$ と表せるので、位置ベクトルは次のように変形できます。
>
> $$\vec{CH} = k\vec{CG} \implies \vec{OH} = (1-k)\vec{OC} + k\vec{OG}$$

> **✨ 翻訳ルール②：「点 $H$ は平面 $OAB$ 上にある」**
>
> 平面 $OAB$ 上にあるということは、$\vec{OH}$ を $\vec{a}$ と $\vec{b}$ だけで表現できる（＝基底となる $\vec{c}$ が登場しない）ということです。
>
> つまり、**引用「$\vec{c}$ の係数が 0 になる」** ように上の式を整理すれば、一発で位置ベクトルが確定します。

---

## ✍️ 模範解答

### (1) $\vec{OH}$ を $\vec{a}, \vec{b}$ を用いて表す

点 $P, Q, R$ の定義より、

$$
\vec{OP} = \frac{1}{2}\vec{a}, \quad \vec{OQ} = \frac{2}{3}\vec{b}, \quad \vec{OR} = \frac{3}{4}\vec{c}
$$

$G$ は $\triangle PQR$ の重心なので、

$$
\vec{OG} = \frac{\vec{OP} + \vec{OQ} + \vec{OR}}{3} = \frac{1}{6}\vec{a} + \frac{2}{9}\vec{b} + \frac{1}{4}\vec{c}
$$

点 $H$ は直線 $CG$ 上にあるので、実数 $k$ を用いて $\vec{CH} = k\vec{CG}$ と表せる。

$$
\begin{aligned}
\vec{OH} &= (1-k)\vec{c} + k\vec{OG} \\
&= \frac{k}{6}\vec{a} + \frac{2k}{9}\vec{b} + \left(1 - \frac{3}{4}k\right)\vec{c}
\end{aligned}
$$

ここで、点 $H$ は平面 $OAB$ 上にあるため、$\vec{c}$ の係数は $0$ となる。

$$
1 - \frac{3}{4}k = 0 \implies k = \frac{4}{3}
$$

これを代入して、求める位置ベクトルは、

$$
\vec{OH} = \frac{2}{9}\vec{a} + \frac{8}{27}\vec{b}
$$

---

### (2) $|\vec{a}|, |\vec{b}|$ を求める

直線 $CH$ と平面 $OAB$ は垂直なので、$\vec{CH} \perp \vec{a}$ かつ $\vec{CH} \perp \vec{b}$ が成り立つ。すなわち内積が $0$。

$$
\vec{CH} = \vec{OH} - \vec{OC} = \frac{2}{9}\vec{a} + \frac{8}{27}\vec{b} - \vec{c}
$$

$\vec{CH} \cdot \vec{a} = 0$ より、

$$
\frac{2}{9}|\vec{a}|^2 + \frac{8}{27}(\vec{b}\cdot\vec{a}) - (\vec{c}\cdot\vec{a}) = 0
$$

与えられた条件 $\vec{a}\cdot\vec{b}=3, \vec{c}\cdot\vec{a}=1$ を代入すると、

$$
\frac{2}{9}|\vec{a}|^2 + \frac{8}{27}(3) - 1 = 0 \implies \frac{2}{9}|\vec{a}|^2 = \frac{1}{9} \implies |\vec{a}| = \frac{1}{\sqrt{2}}
$$

同様に、$\vec{CH} \cdot \vec{b} = 0$ Loy、

$$
\frac{2}{9}(\vec{a}\cdot\vec{b}) + \frac{8}{27}|\vec{b}|^2 - (\vec{c}\cdot\vec{b}) = 0
$$

条件 $\vec{a}\cdot\vec{b}=3, \vec{b}\cdot\vec{c}=9$ を代入すると、

$$
\frac{2}{9}(3) + \frac{8}{27}|\vec{b}|^2 - 9 = 0 \implies \frac{8}{27}|\vec{b}|^2 = \frac{25}{3} \implies |\vec{b}|^2 = \frac{225}{8} \implies |\vec{b}| = \frac{15\sqrt{2}}{4}
$$

---

### (3) $\triangle OAB$ の面積 $S$

三角形の面積公式より、

$$
\begin{aligned}
S &= \frac{1}{2}\sqrt{|\vec{a}|^2|\vec{b}|^2 - (\vec{a}\cdot\vec{b})^2} \\
&= \frac{1}{2}\sqrt{\left(\frac{1}{2}\right)\left(\frac{225}{8}\right) - 3^2} \\
&= \frac{1}{2}\sqrt{\frac{225}{16} - \frac{144}{16}} = \frac{1}{2}\sqrt{\frac{81}{16}} = \frac{1}{2} \cdot \frac{9}{4} = \frac{9}{8}
\end{aligned}
$$

---

### (4) 四面体 $OABC$ の体積 $V$

四面体の高さは、垂直な線分 $CH$ の長さ $|\vec{CH}|$ に等しい。

$$
\begin{aligned}
|\vec{CH}|^2 &= \left|\frac{2}{9}\vec{a} + \frac{8}{27}\vec{b} - \vec{c}\right|^2 \\
&= \frac{4}{81}|\vec{a}|^2 + \frac{64}{729}|\vec{b}|^2 + |\vec{c}|^2 + \frac{32}{243}(\vec{a}\cdot\vec{b}) - \frac{16}{27}(\vec{b}\cdot\vec{c}) - \frac{4}{9}(\vec{c}\cdot\vec{a})
\end{aligned}
$$

ここにすべての値を代入して慎重に計算すると、

$$
|\vec{CH}|^2 = \frac{1}{9} \implies |\vec{CH}| = \frac{1}{3}
$$

よって、求める体積 $V$ は、

$$
V = \frac{1}{3} \times \triangle OAB \times |\vec{CH}| = \frac{1}{3} \times \frac{9}{8} \times \frac{1}{3} = \frac{1}{8}
$$

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
    .ksq-btn-title { white-space:normal; }
    .ksq-trust .sep { display:none; }
  }
  @container (max-width: 600px) {
    .ksq-cta-inner { padding:36px 20px; }
    .ksq-eyebrow { margin-bottom:28px; gap:8px; }
    .ksq-wordmark { font-size:19px; }
    .ksq-num { font-size:56px; }
    .ksq-num-label { font-size:15px; letter-spacing:0.14em; }
    .ksq-tag { font-size:28px; letter-spacing:0.05em; margin-top:-40px; margin-bottom:12px; }
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
      <p class="ksq-body">学校や集団塾ではしてくれない、志望大学の過去問<strong style="color:#0b2240;">10年単位の研究</strong>に基づくオーダーメイドのカリキュラム。最難関大合格講師が、あなただけの合格ロードマップを直接設計します。</p>
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