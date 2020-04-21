.. |br| raw:: html

   <br />

Custom Content Types
===========================

Brief Background for Custom Content Types
------------------------------------------
From the very early versions of Drupal, the concept of a ``node`` was central to how content management was handled.
Originally the node was used for various entities like articles and blog pages. Over time, the node was
adapted for many other uses by the ability to attach many different field types to a node, like file attachments or
datetime fields. In Drupal 8, this concept of adding different fields (or being ``fieldable``) was extended to
many more entities like taxonomies, users and blocks as well.

In many ways, however, the node is still the most flexible of content types in Drupal. It is usually the easiest
to work with because it has the most mature set of integrations with the underlying CMS. Currently we find extending
the node with appropriate fields is entirely adequate as well as the simplest approach in many cases, so this is the
approach that we often take in this version of our demo Drupal ELN (``MyLabBook``).

Custom Content Types in MyLabBook
------------------------------------
When we extend the basic node entity by attaching different fields, we are creating a new type of
node, which is often referred to as a ``Custom Content Type`` (also referred to sometimes as a ``Node Bundle``).
For MyLabBook, at this point we have only two Custom Content Types, the Experiment and the Protocol Step.

Custom Content Type of an Experiment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The Experiment custom content type stores the metadata for the experiment along with acting as a container for
all of the protocol steps in the experiment.

Custom Content Type of a Protocol Step
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
The heart of MyLabBook is the Protocol Step custom content type. It is these protocol steps that make up the
steps in an experiment. They could also have been called an Experimental Step, but in most cases during an
experiment the researcher is following or developing some type of protocol. For that reason and to ease problems with
namespace collision, the name of Protocol Step is used instead. This is also consistent with the nomenclature
used by other ELNs.

Each Protocol Step contains the fields that are needed for the given step of the experiment. There are a few
different approaches that may come to mind for creating a basic Protocol Step custom content type.

   * Create one Protocol Step custom content type that has all of the fields that you will need for any step that
     you have in your experiment. Then use that Protocol Step for each step in your experiment, leaving fields blank
     if they are not needed.
   * Create multiple different Protocol Step custom content types, one custom content type for each different type of
     step that you need. Then use the appropriate Protocol Step custom content type for a given step in your
     experiment.
   * Use a hybrid approach between the first and second approach, so that you have a few Protocol Step custom
     content types and use the Protocol Step type that best fits your given experimental step, with a few of the
     different fields perhaps left blank in a given step.

In this first version of MyLabBook, we have taken the first approach for simplicity, but good cases can be made for
the second and third approaches as well.

Tabs for Protocol Step Field Sets
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Since we take the first approach for the Protocol Step of including *all* of the possible fields, then we also
want to hide unused fields from the interface as much as possible so that the interface does not become too confusing.
In this version of MyLabBook we use tabs for each set of fields, and then there are checkboxes for hiding or
displaying the tabs of interest for a given Protocol Step.

The following tabs are available for a Protocol Step, with each tab displaying one or more fields for that tab.

    * Task List
    * Rich Text Notes
    * Tables or Grids for Data
    * Geolocation Address and Coordnates (Lat & Long)
    * Image and File Uploads
    * Web Site URLs and descriptors
    * Sets of Labels with Decimal Values
    * Sets of Labels with Integer Values
    * Sets of Labels with Floating Point Values
    * Sets of Labels with Text Values
    * Sets of Labels with Date Values
    * Uploaded Videos or Embedded YouTube Videos

This combination of hiding unused tabs along with having many different types of field sets to choose from should
allow researchers in most cases to customize a given Protocol Step to reflect their needs for an appropriate set of
data to collect.






