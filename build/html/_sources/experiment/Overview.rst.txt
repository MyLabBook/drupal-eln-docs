.. |br| raw:: html

   <br />

.. _overview-of-an-experiment:

Overview of an Experiment
======================================

.. admonition:: Good References for Custom Content Types

   *  `Working with content types and fields <https://www.drupal.org/docs/8/administering-drupal-8-site/managing-content-0/working-with-content-types-and-fields/>`_ :
      Overview of how fields are used with custom content types
   *  `Adding Content And Content Types <https://www.sooperthemes.com/drupal-blog/adding-content-and-content-types-drupal-8-8-days-drupal-8-day-4>`_ :
      Part of a tutorial from SooperThemes that describes how to add fields to custom content types

As mentioned in :ref:`experiments-in-a-drupal-eln`, the Experiment custom content type contains fields that correspond
to the experiment as a whole. These fields parallel the fields used in the
`protocols.io website <https://protocols.io>`_ for an experiment to a large extent.

For those wishing to change
these fields (i.e., add, remove or modify the fields), then after logging in as an administrator,
the Experiment custom content type can be changed from the
``Structure >> Content types >> Experiment >> Manage Fields`` administrative area. More information is available
from the references listed at the beginning of this section.

Tabs and Fields
-------------------
There are 5 tabs that are displayed for a given experiment, and for each tab there are several different
fields that may be populated and displayed. These tabs (highlighted in blue) and the field under each tab are
listed below.

    * Overview
        * **Researchers** - Names of one or more researchers involved in this experiment
        * **Organizations** - Organizations of the researchers or organizations that were somehow involved in this
          research
        * **Images** - Images that might pertain to this research as a whole (there is also a field where images
          can be attached to each Protocol Step as well).
    * Preliminaries
        * **Preparation** - What type of preparation should be done for this experiment
        * **Guidelines** - The set of guidelines or standards to use in this experiment
        * **Safety Warnings** - This should describe any safety precautions that should be made for this experiment
    * Scientific Method
        * **Hypothesis** - The scientific hypothesis that describes the purpose of this experiment
        * **Conclusion** - The conclusion that can be made from this experiment, especially in regards to the
          original hypothesis
    * Relevant Docs & Websites
        * **Relevant Documents** - One or more documents (e.g., pdf, docx) that are relevant
          to this experiment can be uploaded and each document can be given a title.
        * **Relevant Websites** - One or more URLs can be added, with each URL given a name or title
    * Metadata
        * **Keywords** - List of keywords associated to this experiment
        * **License** - The license for the intellectual property of this experiment
        * **DOI** - Digital Object Identifier used to permanently identify an article or document on the web
        * **Citation** - How to cite this experiment or protocol in research papers

