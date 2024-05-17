---
title: Probability of Drawing Red Socks
date: 2024-05-17
categories: [Probability]
tag: [fifty]
---

<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Probability of Drawing Red Socks</title>
  <style>
    .boxed {
      border: 1px solid black;
      padding: 10px;
      margin-bottom: 20px;
    }
    .centered-heading {
      text-align: center;
      font-weight: bold;
      font-size: 1.5em;
      margin-bottom: 20px;
    }
  </style>
  <script type="text/javascript" async
    src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML">
  </script>
  <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
      tex2jax: {
        inlineMath: [['$', '$'], ['\\(', '\\)']],
        displayMath: [['$$', '$$'], ['\\[', '\\]']],
        processEscapes: true
      }
    });
  </script>
</head>
<body>
  <div class="centered-heading">Probability of Drawing Red Socks</div>
  <div class="boxed">
    <p>A drawer contains red socks and black socks. When two socks are drawn at random, the probability that both are red is \( \frac{1}{2} \). (a) How small can the number of socks in the drawer be? (b) How small if the number of black socks is even?</p>
  </div>
  <p>Let us begin by making the reasonable assumption that each draw is independent. Then let</p>
  <ol>
    <li>\( R \) : denotes the event of drawing a red sock</li>
    <li>\( r \) and \( b \) denote the number of red socks and black socks respectively</li>
  </ol>
  <p>Then it follows that</p>
  <p>$$ \mathbf{Pr}(R,R) = \frac{r}{r+b}\frac{r-1}{r+b-1} $$</p>
  <p>Then it is easy to see that if you have four socks in total with 3 red and 1 black, then \( \mathbf{P}(r,r) = \frac{3}{4}\frac{2}{3} = \frac{1}{2} \). Furthermore, note that if there were 2 red and 2 black then \( \mathbf{Pr}(R,R) = \frac{2}{4}\frac{1}{3} \neq \frac{1}{2} \). We claim this is the minimal case, to see this note that if there is 1 red and 3 black then obviously the drawing two red socks is a probability 0 event. If we have 3 socks in total, then we must have 2 red socks and 1 black sock, otherwise, it is clear that we have either a probability 1 event or a probability 0 event, however in this case note that \( \mathbf{P}(r,r) = \frac{1}{3} \). Furthermore, it is also clear that one cannot have less than 3 socks in total, as if there were only one sock in total then \( \mathbf{P}(r,r) = 0 \), and if there were two socks in total either \( \mathbf{P}(r,r) = 0 \) or \( \mathbf{P}(r,r) = 1 \). Hence the correct answer for part (a) is \( 4 \).</p>
  <p>The answer to part (b) is slightly more complicated. First note that by the above, the pair \( (r,b) \) must satisfy the equation:</p>
  <p>$$ \frac{1}{2} = \frac{r}{r+b}\frac{r-1}{r+b-1} \iff r^2 - r(1+2b) + (b-b^2) = 0 $$</p>
  <p>using the quadratic formula:</p>
  <p>$$ r = \frac{1}{2} + b \pm \frac{1}{2}\sqrt{1 + 8b^2} \tag{1} $$</p>
  <p>and substituting \( b = 2x \) as we demand \( b \) to be even we obtain:</p>
  <p>$$ r = \frac{1}{2}\left[ (1+4x) \pm \sqrt{1 + 32x^2} \right] \tag{2} $$</p>
  <p>we note that \( r \) must be an integer, hence we must have that \( (1+4x) \pm \sqrt{1 + 32x^2} \) is an even integer. The smallest \( x \) to accomplish this is \( x = 3 \) by easy case work, when taking the \( + \) version. Furthermore, it is easy to justify that the correct solution to take is the \( + \) version. To see this recall from the above that \( r = 3 \) and \( b = 1 \) is a valid solution, hence these values should satisfy (1), then \( 3 = 1.5 \pm 1.5 \), hence clearly one must take the adding solution. Therefore, we have that the smallest even number of black socks we can have is \( b = 2x = 6 \) and by (2) this determines the number of red socks we can have, namely \( r = 15 \), thus the smallest total number of socks in the box is \( 21 \).</p>
</body>
</html>
