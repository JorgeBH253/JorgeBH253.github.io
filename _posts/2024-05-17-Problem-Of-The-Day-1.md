---
title: Probability of Drawing Red Socks
date: 2024-05-17
categories: [Probability]
tag: [fifty]
---

# Probability of Drawing Red Socks

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
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-MML-AM_CHTML">
</script>

<div class="centered-heading">Probability of Drawing Red Socks</div>

<div class="boxed">
  A drawer contains red socks and black socks. When two socks are drawn at random, the probability that both are red is \( \frac{1}{2} \). 
  (a) How small can the number of socks in the drawer be? 
  (b) How small if the number of black socks is even?
</div>

Let us begin by making the reasonable assumption that each draw is independent, then it follows that 
\( \mathbf{P}(r,r) = \frac{r}{r+b}\frac{r-1}{r+b-1} \), where \( r \) and \( b \) denote the number of red socks and black socks respectively.

Then it is easy to see that if you have four socks in total with 3 red and 1 black, then 
\( \mathbf{P}(r,r) = \frac{3}{4}\frac{2}{3} = \frac{1}{2} \).

Furthermore, note that if there were 2 red and 2 black, then because the probability of drawing the first red sock is \( \frac{1}{2} \), the total probability cannot be \( \frac{1}{2} \). Similarly, if there were only 1 red and 3 black, then obviously drawing two red socks is a probability 0 event. If we have three socks in total, then we must have 2 red socks and 1 black sock; otherwise, it is clear that we have either a probability one event or a probability 0 event. However, in this case, note that 
\( \mathbf{P}(r,r) = \frac{1}{3} \).

Hence the correct answer for part (a) is 4. The answer to part (b) is slightly more complicated. First, note that by the above,

\[ \mathbf{P}(r,r) = \frac{3}{4}\frac{2}{3} = \frac{1}{2} = \frac{1}{2} \]

Hence the correct answer for part (a) is 4. The answer to part (b) is slightly more complicated. First, note that by the above,

\[ \mathbf{P}(r,r) = \frac{3}{4}\frac{2}{3} = \frac{1}{2} = \frac{1}{2} \]
