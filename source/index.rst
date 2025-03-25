.. MGlyph documentation master file, created by
   sphinx-quickstart on Tue Mar 25 10:27:00 2025.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

MGlyph library
==============

Malleable Glyph is a **small graphical design**, fitting exactly to a square of 1in × 1in. It is **"shaped" by a numerical parameter** $x$ ranging from $0.0$ to $100.0$.

This is the `mglyph` library that offers an easy way how to design and preview malleable glyphs:

.. code:: python

   def simple_line(x: float, canvas:mg.Canvas) -> None:
       canvas.line((mg.lerp(x, 0, -1), 0), (mg.lerp(x, 0, 1), 0),
                  width='50p', color='navy', linecap='round')
   mg.show(simple_line)

To start with `mglyph`
========================

* check out `the tutorial <https://github.com/adamherout/mglyph/blob/main/tutorials/mglyph%20tutorial.ipynb>`_ (just download the Jupyter Notebook and run it, or explore the same one `in Google Colab <https://colab.research.google.com/drive/1T8DHWpUBLNbo-QB5o6SXDjZrHjSVp4vv>`_)
* see the library `homepage at GitHub <https://github.com/adamherout/mglyph?tab=readme-ov-file#introduction>`_
* read `the paper <https://arxiv.org/abs/2503.16135>`_

.. toctree::
   :maxdepth: 2
   :caption: Contents
   
   install
   tutorial
   mglyph

