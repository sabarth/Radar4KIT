Basic information about RADAR4KIT
+++++++++++++++++++++++++++++++++

RADAR4KIT allows you to compile research data from completed scientific studies and projects into data packages, 
describe them with metadata, store and archive them permanently, or make them publicly accessible as needed. Published data are assigned a persistent 
identifier (DOI) and can thus be found internationally and are also referenced in `KITopen <https://www.bibliothek.kit.edu/english/kitopen.php>`_ . 
RADAR4KIT represents a generic offer of KIT in addition to the established subject repositories, which can be found e.g. in [re3data.org](re3data.org).

The operator is the `Karlsruhe Institute of Technology <https://kit.edu>`_ (KIT). RADAR4KIT is based on the `RADAR <https://radar.products.fiz-karlsruhe.de/en>`_ 
service offered by FIZ Karlsruhe. The data is stored exclusively on KIT's IT infrastructure at the Steinbuch Centre for Computing (SCC). 


Registration and user profiles
==============================

Since RADAR4KIT is an online service it can be used exclusively via the Internet. All KIT researchers can log in to RADAR4KIT via their KIT account (Shibboleth) using 
the web frontend of `RADAR4KIT <www.radar.kit.edu>`_. In addition, further accounts for KIT-externals can be created in special cases. 

.. image:: /images/radar4kit_edit_metadata_1.png


RADAR4KIT usage and numbers
===========================

RADAR4KIT can be used via a web-based user interface with current web browsers or via the REST-based `RADAR API <https://radar.products.fiz-karlsruhe.de/de/radarfeatures/radar-api>`_ . The data provider (can be "subcurator" or "curator") can create data packages within the workspace assigned to him and assign individual files or file archives (.tar, .zip, .tgz, tar.gz, .tar.bz2) containing multiple files. The data provider also can add or delete individual data via the user interface. With RADAR4KIT the **maximum files size is at about 200GB** for archiving and publishing data. The 200GB refers to both single or multiple files and thus representing the current maximum of possible repository size. However since the **web browsers** start stuggeling on resources at file sizes of **10GB** and more you should use the `RADAR API <https://radar.products.fiz-karlsruhe.de/de/radarfeatures/radar-api>`_ to upload bigger file sizes!

The data provider is also responsible for describing the data packages with proper metadata following certain standards. For this purpose, the service provides a form on the RADAR4KIT platform. Alternatively, it is possible to create the metadata offline as an XML file (see Appendix for an example) and then upload it to the RADAR4KIT platform. The data provider can also use the RADAR4KIT platform to download a template for a corresponding XML file as well as an XML schema for validating the metadata in the latest version. 



Retention period and immutability of data packages
==================================================
RADAR4KIT enables the permanent and secured storage of data packages over a defined period of time ("retention period"). 
For archived data packets, the data provider defines a retention period. The actual retention period for archived data packets may 
be shorter if the RADAR4KIT service is discontinued before the retention period expires. No retention period needs to be selected for 
published data packages because this period is basically unlimited. KIT guarantees an actual retention period of at least 10 years.
During the retention period, RADAR4KIT does not modify the stored data packets any more, but only ensures their physical preservation 
("bitstream preservation"). Accordingly, RADAR4KIT guarantees neither the permanent usability nor the interpretability of the data contained 
in a data package, as these depend on the availability of the data formats selected by the data provider and corresponding programs for their 
interpretation.

Data packages in permanent storage can no longer be modified. Deletions can be carried out by the administrator in justified exceptional cases
after consultation with the operator. Justified exceptional cases include, for example, legal violations or erroneous data. In the case of deletion, 
only the data is deleted, but not the metadata. These will contain a note that the data has been deleted.


Reviewing research data
=======================
RADAR4KIT also supports a review process prior to a data publication. For this purpose, a data package can be set to the status 
"under review" before publication. In this state, the data package is no longer editable. RADAR4KIT generates a unique link that 
the data provider can pass on to the responsible publisher or reviewers. This link allows access to the not yet published data package
without prior authentication. After completion of the review, the data provider can either change the status for the work package back to 
edit mode or publish the data package. In both cases, the unique link generated becomes invalid, so reviewers can no longer access the data package. 
The data provider can set a data package to the status "in review" several times in succession. The operator does not carry out any further quality 
assurance of the content of the posted research data. The data providers themselves are responsible for this.


Access system and embargos
===========================

Data packages that have not yet been archived or published, i.e. are in the **processing state**, can only be viewed by the data providers, the curators and the administrators. For peer review, there is an exception for reviewers (see section :ref:`Reviewing research data<Reviewing research data>`). 

* **Archived data packages** are normally accessible only to the data provider and the administrator. The data provider can grant other users registered with RADAR4KIT the right to view the descriptive metadata and retrieve the archived data packages. If desired, he may also make the archived dataset publicly available. These rights assignments can be changed at any time by the data provider. Archived data (unless the data provider has made it publicly accessible in whole or in part) cannot be found via search or via OAI. Third parties cannot view or search the data or the metadata.

* **Published data packages**, as well as archived data packages for which the data provider has set access rights so that they are unrestrictedly publicly accessible, can be accessed by all data users registered with RADAR4KIT and anonymous (non-registered) data users. The descriptive metadata are searchable in the web interface and are also available for harvesting via an `OAI provider <https://www.openarchives.org/service/listproviders.html>`_ (Open Archives Initiative). Furthermore, they are publicly viewable at `www.datacite.org <www.datacite.org>`_. This is true even if the actual research data is still under embargo. The data provider can set up an embargo period of up to 12 months after publication for the actual research data, during which only the metadata can be searched and retrieved, but not the research data. After the embargo period has expired, the research data will also be generally retrievable. 