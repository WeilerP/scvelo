|PyPI| |PyPIDownloads| |Docs|

scVelo - RNA velocity generalized through dynamical modeling
============================================================

.. image:: https://user-images.githubusercontent.com/31883718/67709134-a0989480-f9bd-11e9-8ae6-f6391f5d95a0.png
   :width: 300px
   :align: left

.. include:: _key_contributors.rst

**scVelo** is a scalable toolkit for RNA velocity analysis in single cells; RNA velocity
enables the recovery of directed dynamic information by leveraging splicing kinetics
:cite:p:`LaManno18`. scVelo collects different
methods for inferring RNA velocity using an expectation-maximization framework
:cite:p:`Bergen20` or metabolically labeled transcripts :cite:p:`Weiler24`.

scVelo's key applications
^^^^^^^^^^^^^^^^^^^^^^^^^
- estimate RNA velocity to study cellular dynamics.
- identify putative driver genes and regimes of regulatory changes.
- infer a latent time to reconstruct the temporal sequence of transcriptomic events.
- estimate reaction rates of transcription, splicing and degradation.
- use statistical tests, e.g., to detect different kinetics regimes.


Citing scVelo
^^^^^^^^^^^^^

If you include or rely on scVelo when publishing research, please adhere to the
following citation guide:

**EM and steady-state model**

If you use the *EM* (*dynamical*) or *steady-state model*, cite

.. code-block:: bibtex

    @article{Bergen2020,
        title = {Generalizing RNA velocity to transient cell states through dynamical modeling},
        volume = {38},
        ISSN = {1546-1696},
        url = {http://dx.doi.org/10.1038/s41587-020-0591-3},
        DOI = {10.1038/s41587-020-0591-3},
        number = {12},
        journal = {Nature Biotechnology},
        publisher = {Springer Science and Business Media LLC},
        author = {Bergen, Volker and Lange, Marius and Peidli, Stefan and Wolf, F. Alexander and Theis, Fabian J.},
        year = {2020},
        month = aug,
        pages = {1408-1414}
    }

**RNA velocity inference through metabolic labeling information**

If you use the implemented method for estimating RNA velocity from metabolic labeling
information, cite

.. code-block:: bibtex

    @article{Weiler2024,
        author = {Weiler, Philipp and Lange, Marius and Klein, Michal and Pe'er, Dana and Theis, Fabian},
        publisher = {Springer Science and Business Media LLC},
        url = {http://dx.doi.org/10.1038/s41592-024-02303-9},
        doi = {10.1038/s41592-024-02303-9},
        issn = {1548-7105},
        journal = {Nature Methods},
        month = jun,
        number = {7},
        pages = {1196-1205},
        title = {CellRank 2: unified fate mapping in multiview single-cell data},
        volume = {21},
        year = {2024},
    }

Support
^^^^^^^
Found a bug or would like to see a feature implemented? Feel free to submit an
`issue <https://github.com/theislab/scvelo/issues/new/choose>`_.
Have a question or would like to start a new discussion? Head over to
`GitHub discussions <https://github.com/theislab/scvelo/discussions>`_.
Your help to improve scVelo is highly appreciated.


.. toctree::
   :caption: Main
   :maxdepth: 1
   :hidden:

   about
   installation
   api
   release_notes
   references

.. toctree::
   :caption: Tutorials
   :maxdepth: 1
   :hidden:

   getting_started
   VelocityBasics
   DynamicalModeling
   DifferentialKinetics
   vignettes/index

.. toctree::
   :caption: Perspectives
   :maxdepth: 1
   :hidden:

   perspectives/index


.. |PyPI| image:: https://img.shields.io/pypi/v/scvelo.svg
   :target: https://pypi.org/project/scvelo

.. |PyPIDownloads| image:: https://pepy.tech/badge/scvelo
   :target: https://pepy.tech/project/scvelo

.. |Docs| image:: https://readthedocs.org/projects/scvelo/badge/?version=latest
   :target: https://scvelo.readthedocs.io

.. _Scanpy: https://scanpy.readthedocs.io

.. |br| raw:: html

  <br/>

.. |dim| raw:: html

   <span class="__dimensions_badge_embed__" data-id="pub.1129830274" data-style="small_rectangle"></span>
   <script async src="https://badge.dimensions.ai/badge.js" charset="utf-8"></script>
