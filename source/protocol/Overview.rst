.. |br| raw:: html

   <br />

.. _overview-of-a-protocol-step:

Overview of a Protocol Step
======================================

.. admonition:: Good References for Custom Content Types

   *  `Working with content types and fields <https://www.drupal.org/docs/8/administering-drupal-8-site/managing-content-0/working-with-content-types-and-fields/>`_ :
      Overview of how fields are used with custom content types
   *  `Adding Content And Content Types <https://www.sooperthemes.com/drupal-blog/adding-content-and-content-types-drupal-8-8-days-drupal-8-day-4>`_ :
      Part of a tutorial from SooperThemes that describes how to add fields to custom content types

As mentioned in :ref:`protocol-steps-in-a-drupal-eln`, the Protocol Step custom content type contains fields
that are used for setting the state of the Protocol Step or for collecting data for the Protocol Step.

For those wishing to change
these fields (i.e., add, remove or modify the fields), then after logging in as an administrator,
the Protocol Step custom content type can be changed from the
``Structure >> Content types >> Protocol Step >> Manage Fields`` administrative area. More information is available
from the references listed at the beginning of this section.

Tabs and Fields
-------------------
There are up to 12 tabs that are displayed for a given protocol step, and for each tab there are several different
fields that may be populated and displayed. Each tab has a field for Tab Label and Notes. If set, the Tab Label is
a string that will be displayed as the label or value for this tab if it is visible. If set, the Notes will be
shown just below the tab label. It will only display if it is non-blank.

The tab default names (highlighted in blue) are shown below along with any unique fields for that tab (apart from
the Tab Label and Notes fields).

    * Task List
        * **Task Checklist** - One or more tasks that will be displayed as a list of complete or incomplete tasks
          in the protocol step view. In order to show the task as complete, then the checkbox of this form needs
          to be checked.
    * Notes in Rich Text
        * **Notes** - This is a little different from most other tabs in that this already is for rich text notes.
          The difference here is that as many rich text notes boxes as are needed can be added and will be
          displayed.
    * Data Tables
        * **Data Tables** - This uses the `Table Field module <https://www.drupal.org/project/tablefield>`_ to
          display an HTML table, which can be useful for data collection since it is a free format table.
    * Location
        * **Location Address** - This is the street address of the location being recorded. If it is a valid
          street address, then it will automatically populate the Latitude and Longitude in the Geolocation
          Single area once the protocol step is saved.
        * **Geolocation Single** - This contains the Latitude and Longitude of the location that is to be
          recorded.
    * Image & File Uploads
        * **Protocol Images** - Image files that can be uploaded to the ELN and then will be displayed as images.
        * **Protocol Files** - Usually some sort of document files that can be uploaded to the ELN. Usually these
          are shown as links in the display of the Drupal ELN.
    * Web Sites
        * **URL** - One or more URLs in the list of websites. Each URL is accompanied by a Link Text value for the
          display of the URL.
    * Decimal Values
        * **Decimal Values** - This uses the `Double Field module <https://www.drupal.org/project/double_field>`_ to
          create a list of one or more dual field sets, with each set having both a text label field matched with a
          decimal field.
    * Integer Values
        * **Integer Values** - This uses the `Double Field module <https://www.drupal.org/project/double_field>`_ to
          create a list of one or more dual field sets, with each set having both a text label field matched with an
          integer field.
    * Float Values
        * **Float Values** - This uses the `Double Field module <https://www.drupal.org/project/double_field>`_ to
          create a list of one or more dual field sets, with each set having both a text label field matched with a
          floating point field.
    * Text Values
        * **Text Values** - This uses the `Double Field module <https://www.drupal.org/project/double_field>`_ to
          create a list of one or more dual field sets, with each set having both a text label field matched with a
          text field as a value.
    * Date Values
        * **Date Values** - This uses the `Double Field module <https://www.drupal.org/project/double_field>`_ to
          create a list of one or more dual field sets, with each set having both a text label field matched with a
          date field.
    * Videos
        * **Use Existing Media** - This allows you to upload your own video files (in mp4 format) to the media
          list and then use the look-ahead text box to enter the title of the uploaded video file.
          This can be done for multiple existing media files that you might want to display for view.
        * **Embedded Videos** - This allows you to embed one or more YouTube videos under this tab.

