---
layout: page
title: Parallelized String Art
description: A parallelized string art solver in C++ and CUDA that computes the string art best resembling the input image
img: assets/img/string-art-icon.jpeg
importance: 3
---


<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/string-art-results" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
String art is an image solely composed of strings between pins around a circular canvas. We implemented a parallelized string art solver in C++ and CUDA that computes the string art best resembling the input image. We developed our algorithm from scratch based on the sequential greedy approach proposed in paper by Brisak et al. We modified the proposed algorithm while implementing our sequential version of the solver, so that algorithm would have more parallelism to exploit while outputting more accurate string art image. We then developed our parallel version of the solver, which produces the same output as the sequential solver in a considerably shorter runtime. We were able to achieve an over 221x speedup on a 512*512 image with 128 pins. For implementation details and performance analysis, see report linked above.

For more information, please checkout the [project page](https://nanxili.github.io/15418-threadart/), the [writeup](https://nanxili.github.io/15418-threadart/pdf/finalReport.pdf), and the [source code](https://github.com/nanxili/15418-threadart/tree/master).