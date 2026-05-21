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

## 📊 過去問研究データ：横国の出題ヒートマップ

なぜ、この空間ベクトルを完璧にする必要があるのか。その理由は、こちらの過去問分析データにあります。

![横国数学ヒートマップ](/images/yokokokurikei.png)


横国の理系数学において、空間ベクトルは微分積分と並ぶ「超・最頻出分野」です。特に「直線と平面の交点」や「垂直条件（内積＝0）を利用した計量」は、形を変えて何度も出題されています。

ここをスムーズに解き切れるかどうかが、横国理系キャンパスへの切符を握っています。

---

## 💡 発想のポイント：日本語を「数学語（数式）」に翻訳せよ

空間ベクトルが苦手な人は、問題文の日本語をどう数式にすればいいかで迷ってしまいます。
この問題を攻略するための「翻訳ルール」は以下の2つだけです。

### 1. 「点 $H$ は直線 $CG$ 上にある」
直線上の点ということは、実数 $k$ を用いて次のように表せます。
$$
\vec{CH} = k\vec{CG} \implies \vec{OH} = (1-k)\vec{OC} + k\vec{OG}
$$

### 2. 「点 $H$ は平面 $OAB$ 上にある」
平面 $OAB$ 上にあるということは、$\vec{OH}$ を $\vec{a}$ と $\vec{b}$ だけで表現できるということです。
つまり、**「$\vec{c}$ の係数が $0$ になる」** ように上の式を整理すれば、一発で位置ベクトルが確定します。

---

## ✍️ 解答・解説

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

直線 $CH$ と平面 $OAB$ は垂直なので、$\vec{CH} \perp \vec{a}$ かつ $\vec{CH} \perp \vec{b}$ が成り立つ。（すなわち内積が $0$）
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
同様に、$\vec{CH} \cdot \vec{b} = 0$ より、
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

## 🚀 「過去問で点数が取れる」実感を、あなたに。

今回の横国の空間ベクトル、あなたはどこまで迷わずに方針を立て、正確に計算しきることができたでしょうか？

「解説を読めば理解できるけれど、初見でこの計算を合わせる自信がない…」
「志望校の過去問に特化した対策って、何をすればいいのか分からない」

学校や大規模な集団塾では、一人ひとりの志望校の過去問を10年単位で細かく研究し、そこから逆算したカリキュラムまで作ってくれることはほぼありません。

<div style="background-color: #f0f7ff; border: 2px solid #002147; border-radius: 10px; padding: 25px; text-align: center; margin-top: 30px; box-shadow: 0 4px 6px rgba(0,0,0,0.1);">
  <h3 style="color: #002147; margin-top: 0; font-size: 1.4em;">Ksquare「志望校特化塾」</h3>
  <p style="text-align: left; line-height: 1.6; color: #333;">
    Ksquareでは、学校や集団塾ではしてくれない、<strong>あなたの志望大学の過去問10年単位の研究に基づく完全オーダーメイドのカリキュラム</strong>で指導を行います。<br><br>
    あなただけの「志望校特化型・合格ロードマップ」を最難関大学合格講師が直接設計。基礎固めから過去問演習まで、一切の迷いなくスムーズに接続し、<strong>「過去問で確実に点数が取れる」</strong>圧倒的な実感を授けます。
  </p>
  
  <p style="font-weight: bold; color: #e53e3e; font-size: 1.1em; margin-top: 20px;">
    ＼ 志望校特化の戦略で、逆転合格のルートを掴め ／
  </p>

  <a href="https://ksquare-sys.github.io/Ksquare/" style="display: inline-block; background-color: #002147; color: #ffffff; font-size: 1.2em; font-weight: bold; text-decoration: none; padding: 16px 40px; border-radius: 50px; margin-top: 10px; box-shadow: 0 4px 10px rgba(0, 33, 71, 0.4); transition: transform 0.2s;">
    無料戦略診断（面談）を予約する ＞
  </a>
  <p style="font-size: 0.85em; color: #666; margin-top: 12px;">※質の高い指導を維持するため、毎月の受け入れ人数には上限がございます。</p>
</div>