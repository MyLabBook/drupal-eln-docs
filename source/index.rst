.. DrupalELN documentation master file
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

.. |br| raw:: html

   <br />


A Drupal Based Electronic Lab Notebook
========================================
This documentation covers primarily one way to build an Electronic Lab Notebook (ELN)
based on the `Drupal Content Management System <https://www.drupal.org>`_.
This documentation should be hosted at the `MyLabBook.org website <https://www.mylabbook.org>`_ and
the source of the documentation should be available on the associated
`GitHub repository <https://github.com/MyLabBook>`_.

While there are numerous options for building a Drupal based ELN, this documentation focuses on a basic
architecture that uses the following.

   * The core standard installation of Drupal
   * Some contributed modules available on drupal.org
   * Some custom content types based on Drupal nodes
   * A few custom modules that we have developed and plan to host on Drupal.org in the near future

Details are covered in the other sections of this documentation.

The MyLabBook Demo
--------------------
The demo version of a Drupal ELN whose source is found in our `GitHub repository <https://github.com/MyLabBook>`_
is called ``MyLabBook``. Oftentimes throughout this documentation we may use the notion of a Drupal based ELN
and ``MyLabBook`` interchangeably because the ``MyLabBook`` demo is currently the focus
for this documentation. One of the beauties of using a Drupal based ELN is that there could
be many different approaches and many variations on a given approach. This documentation is most appropriate
for those wanting to take the approach we have taken with ``MyLabBook`` or some variation of that approach,
however. If someone wants to take a different approach to building a Drupal based ELN then this documentation may
be helpful in some fashion as well.

This documentation should also be helpful for those wanting to better understand the standard Drupal based ELNs
that are supported on the commercial cloud provider at `MyLabBook.com <https://www.mylabbook.com>`_.

We hope to continue to expand upon these thoughts to make ELNs more accessible and available to researchers,
laboratory administrators, faculty and citizen scientists.
Please feel free to extend this documentation by contributing pull requests at the
`GitHub repository <https://github.com/MyLabBook>`_.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   introduction/index
   experiment/index
   protocol/index


Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
