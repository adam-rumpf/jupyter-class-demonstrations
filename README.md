# Jupyter Notebook Class Demonstrations

<a href="https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD?urlpath=voila%2Frender%2Findex.ipynb"><img src="https://img.shields.io/badge/launch-voil%C3%A0-5dbcaf"/></a> <a href="https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD?filepath=index.ipynb"><img src="https://mybinder.org/badge_logo.svg"/></a> <a href="https://github.com/adam-rumpf/jupyter-class-demonstrations/search?l=jupyter-notebook"><img src="https://img.shields.io/badge/language-jupyter_notebook-blue?logo=jupyter&logoColor=white"/></a> <a href="https://github.com/adam-rumpf/jupyter-class-demonstrations/blob/main/LICENSE"><img src="https://img.shields.io/github/license/adam-rumpf/jupyter-class-demonstrations"/></a> <a href="https://github.com/adam-rumpf/jupyter-class-demonstrations/commits/main"><img src="https://img.shields.io/maintenance/yes/2021"/></a>

A collection of interactive Jupyter Notebook mathematical demonstrations. This is meant as a follow-up to my [Mathematica Class Demonstrations](https://github.com/adam-rumpf/mathematica-class-demonstrations) project, remade using Jupyter Notebooks for ease of access. See the author's page [here](https://adam-rumpf.github.io/demos/jupyter.html).

## Table of Contents

* [Overview](#overview)
* [Calculus, Differential Equations, and Analysis](#calculus-differential-equations-and-analysis)
  * [Cobwebbing](#cobwebbing)
  * [Taylor Series Approximations](#taylor-series-approximations)

## Overview

This repository contains a collection of Jupyter Notebooks written for use as class aids. It is a continuation of my [Mathematica Class Demonstrations](https://github.com/adam-rumpf/mathematica-class-demonstrations) project, remade in a format that does not require the user to own any specialized software.

These notebooks are meant to act as standalone demonstrations that do not require any programming or technical knowledge on the part of the user. All of the links below are to standalone web app versions of the notebooks rendered using [Voil??](https://github.com/voila-dashboards/voila), meaning that the source code remains hidden and the page acts much like a textbook page with interactive widgets. If you wish to view or edit the source code while playing with the widgets you can use the [Binder](https://mybinder.org/) link at the top of this README.

## Calculus, Differential Equations, and Analysis

Many of the files in this folder are based on Mathematica demos originally written to show to my calculus students, either demonstrating material from class or demonstrating material from later classes that indirectly involve the concepts from basic calculus. In particular I find a lot of inspiration from dynamical systems, since they lend themselves quite well to visually demonstrating concepts from calculus.

### Cobwebbing

<img src="img/cobwebbing-chaos.png" height="300"/>

Created 4/20/2021  
[Complete Demonstration](https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD?urlpath=voila%2Frender%2Fcalc-diffeq-analysis%2Fcobwebbing.ipynb)  
[Standalone Widget](https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD?urlpath=voila%2Frender%2Fcalc-diffeq-analysis%2Fcobwebbing-standalone.ipynb)  
[Original Mathematica Demonstration](https://github.com/adam-rumpf/mathematica-class-demonstrations#cobwebbing)

This demonstration gives a brief introduction to [cobwebbing](https://en.wikipedia.org/wiki/Cobweb_plot), a graphical technique for quickly approximating the general behavior of a discrete dynamical system. This is a useful technique in mathematical biology since many population growth models take the form of a difference equation. In particular, if the population in the next time step is given as a function _f_ of the population in the current time step, then the cobweb plot can be used to estimate the sequence of population values over many time steps by drawing a zig-zagging line alternately between the _y = f(x)_ curve and the _y = x_ line. The complete demonstration includes an explanation for the motivation behind cobweb diagrams and the reasoning behind why they work, and goes through a few population models as examples. The standalone version includes only a pair of interactive widgets showing the process of drawing cobweb plots for two systems with adjustable parameters.

### Taylor Series Approximations

<img src="img/taylor-series-bell.png" height="300"/> <img src="img/taylor-series-sine.png" height="300"/>

Created 4/17/2021  
[Complete Demonstration](https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD?urlpath=voila%2Frender%2Fcalc-diffeq-analysis%2Ftaylor-series.ipynb)  
[Standalone Widget](https://mybinder.org/v2/gh/adam-rumpf/jupyter-class-demonstrations/HEAD?urlpath=voila%2Frender%2Fcalc-diffeq-analysis%2Ftaylor-series-standalone.ipynb)  
[Original Mathematica Demonstration](https://github.com/adam-rumpf/mathematica-class-demonstrations#taylor-and-fourier-series-approximations)

This demonstration shows how a [Taylor series](https://en.wikipedia.org/wiki/Taylor_series) approximation of a given function changes as more terms are added to the series. The complete demonstration includes a mini-lesson showing how the Taylor series can be arrived at by building up a sequence of increasingly-complicated polynomial approximations, while the standalone widget includes only the final widget for manipulating the center and degree of the approximation for a variety of test functions. These can be used to show how well the approximations model the original function near or far from the center, and how adding more terms changes things.
