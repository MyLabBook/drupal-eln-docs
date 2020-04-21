.. |br| raw:: html

   <br />

Contrib Modules
=====================
The thousands of modules that are available on the drupal.org website are usually referred to in the Drupal
community as ``contrib modules``, which is short for ``contributed modules``. The contrib modules
that are used in this version of MyLabBook are described below.

Double field
-------------
The `double field module <https://www.drupal.org/project/double_field>`_ has great possibilities for use in
an ELN. It provides the ability to match up two different field types and basically treat them as one field type.
The following sub-field types can be used in these match-ups.

   * Boolean
   * Text
   * Text (long)
   * Integer
   * Float
   * Decimal
   * Email
   * Telephone
   * Date
   * Url

At a very basic level a label (text field) can be coupled with any of these other fields to collect data of
one of the types shown above. With Drupal it is also easy to designate whether these double fields are a list of
double fields or just one double field.

In this version of MyLabBook, we use this module fairly extensively.

    * Boolean Double Field with HTML enabled text for a Task List
    * Decimal Double Field with a text label a table of decimal values
    * Integer Double Field with a text label a table of integer values
    * Float Double Field with a text label a table of floating point values
    * Text Double Field with a text label a table of text values
    * Date Double Field with a text label a table of date values

Geolocation
--------------
The `geolocation module <https://www.drupal.org/project/geolocation>`_ can also be added to any protocol step to
add fields for geolocation. The most obvious use case for this is when you may be collecting data where the location
of the data point is important. For example, when collecting environmental samples of some type this may be critical.
This module already has capabilities for mapping built in as well. This seems to be a unique ability of MyLabBook as
compared with most other open source ELNs.

Address
--------------
The `address module <https://www.drupal.org/project/address>`_ can be used in conjunction with the Geolocation
module for easy lookup of latitude and longitude values.

Tablefield
-----------
The `tablefield module <https://www.drupal.org/project/tablefield>`_ is another very useful field for an ELN.
It provides a simple table structure with the ability to designate the number of rows and columns in the table.
As with most field types, when the tablefield is added to the Protocol Step custom content type, then the count of
the fields can be designated. So, you can add one table, two tables or unlimited tables to a given step according
to what is most appropriate.

Video Embed
--------------
The `video embed field module <https://www.drupal.org/project/video_embed_field>`_ can be used
to embed YouTube or Vimeo videos. In the MyLabBook demo, only the ability for YouTube embeds is enabled
by default.

Standard Field Types
-----------------------
In addition, we use the following field types that are included in every standard Drupal installation.

    * Entity Reference
    * File Uploads
    * Image Uploads
    * Text (Formatted Long)
    * Text
    * URI / Web Links



