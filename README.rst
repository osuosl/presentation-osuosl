FOSS Hosting at the OSU Open Source Lab
=======================================

This is a slide deck which summarizes the current state of the Open Source Lab.
It uses `Hieroglyph`_ which utilizes ReStructured Text with Sphinx to create
HTML5 slides.

.. _Hieroglyph: http://docs.hieroglyph.io/en/latest/

Howto build the slides
----------------------

Requirements: ``virtualenv`` and ``pip`` plus ``gcc``.

::

  virtualenv venv
  source venv/bin/activate
  pip install -r requirements.txt
  make slides
