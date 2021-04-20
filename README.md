# Jupyter Notebook Class Demonstrations

<a href="https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD"><img src="https://mybinder.org/badge_logo.svg"/></a> <a href="https://github.com/adam-rumpf/jupyter-class-demonstrations/search?l=jupyter-notebook"><img src="https://img.shields.io/badge/language-jupyter_notebook-blue?logo=jupyter&logoColor=white"/></a> <a href="https://github.com/adam-rumpf/jupyter-class-demonstrations/blob/main/LICENSE"><img src="https://img.shields.io/github/license/adam-rumpf/jupyter-class-demonstrations"/></a> <a href="https://github.com/adam-rumpf/jupyter-class-demonstrations/commits/main"><img src="https://img.shields.io/maintenance/yes/2021"/></a>

A collection of interactive Jupyter Notebook mathematical demonstrations. This is meant as a follow-up to my [Mathematica Class Demonstrations](https://github.com/adam-rumpf/mathematica-class-demonstrations) project, remade using Jupyter Notebooks for ease of access.

_This is a work in progress. A full description of the project, along with links to the pages, will be added after a few preliminary demonstrations are complete._

## Table of Contents

* [Overview](#overview)
* [Calculus, Differential Equations, and Analysis](#calculus-differential-equations-and-analysis)
  * [Cobwebbing](#cobwebbing)
  * [Taylor Series Approximations](#taylor-series-approximations)

## Overview

This repository contains a collection of Jupyter Notebooks written for use as class aids. It is a continuation of my [Mathematica Class Demonstrations](https://github.com/adam-rumpf/mathematica-class-demonstrations) project, remade in a format that does not require the user to own any specialized software.

These notebooks are meant to act as standalone demonstrations that do not require any programming or technical knowledge on the part of the user. All of the links below are to standalone web app versions of the notebooks rendered using [Voilà](https://github.com/voila-dashboards/voila), meaning that the source code remains hidden and the page acts much like a textbook page with interactive widgets. If you wish to view or edit the source code while playing with the widgets you can use the [Binder](https://mybinder.org/) link at the top of this README.

## Calculus, Differential Equations, and Analysis

Many of the files in this folder are based on Mathematica demos originally written to show to my calculus students, either demonstrating material from class or demonstrating material from later classes that indirectly involve the concepts from basic calculus. In particular I find a lot of inspiration from dynamical systems, since they lend themselves quite well to visually demonstrating concepts from calculus.

### Cobwebbing

_(Images.)_

Created 4/20/2021

[Complete Demonstration](https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD?urlpath=voila%2Frender%2Fcalc-diffeq-analysis%2Fcobwebbing.ipynb)

[Standalone Widget](https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD?urlpath=voila%2Frender%2Fcalc-diffeq-analysis%2Fcobwebbing-standalone.ipynb)

[Original Mathematica Demonstration](https://github.com/adam-rumpf/mathematica-class-demonstrations#cobwebbing)

_[Cobwebbing](https://en.wikipedia.org/wiki/Cobweb_plot) is a graphical technique for evaluating the long-term behavior of a discrete dynamical system. This demonstration automatically generates cobweb plots for a variety of test systems, although the method is meant to be used by hand to quickly analyze such a system without the need for a computer._

_Specifically, cobwebbing is used for discrete dynamical systems for which the next iteration is given as a function f of the previous iteration. We first plot both the function and the y = x line on the same set of axes. Given an initial value x0, the next value should be f(x0), which we can eyeball from the plot by drawing a vertical line up from x0 on the x-axis until it touches the function curve. Intuitively, if we wanted to find the next iteration, we would need to transfer this value back onto the x-axis and then draw another vertical line up from it. However, because we already have the y = x line drawn, if we simply draw a horizontal line from our current position to it we will automatically reach the x-coordinate corresponding to our current y-coordinate. Then we can simply move vertically from this location. This process can be repeated as many times as needed to approximate the sequence of values produced by the system, alternating between moving vertically to the f curve to evaluate the update step, and then horizontally to the y = x line to convert the y-coordinate to an x-coordinate._

_The points where the function curve passes through the y = x line are the fixed points of the system, and in general an initial solution will either approach or diverge from certain fixed points (or possibly enter a periodic orbit around them), which is how the long-term behavior of the system can be estimated. The result often ends up creating stair-step or spiral patterns which look like cobwebs, hence the name. In chaotic systems, like the [discrete logistic map](https://en.wikipedia.org/wiki/Logistic_map) with large growth rates, it provites a very clear picture of how complicated and messy things can get._

### Taylor Series Approximations

<img src="img/taylor-series-bell.png" height="300"/> <img src="img/taylor-series-sine.png" height="300"/>

Created 4/17/2021

[Complete Demonstration](https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD?urlpath=voila%2Frender%2Fcalc-diffeq-analysis%2Ftaylor-series.ipynb)

[Standalone Widget](https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD?urlpath=voila%2Frender%2Fcalc-diffeq-analysis%2Ftaylor-series-standalone.ipynb)

[Original Mathematica Demonstration](https://github.com/adam-rumpf/mathematica-class-demonstrations#taylor-and-fourier-series-approximations)

This demonstration shows how a [Taylor series](https://en.wikipedia.org/wiki/Taylor_series) approximation of a given function changes as more terms are added to the series. The complete demonstration includes a mini-lesson showing how the Taylor series can be arrived at by building up a sequence of increasingly-complicated polynomial approximations, while the standalone widget includes only the final widget for manipulating the center and degree of the approximation for a variety of test functions. These can be used to show how well the approximations model the original function near or far from the center, and how adding more terms changes things.
