.. _transactions:

Transactions
============

pygeoapi supports the `OGC API - Features - Part 4: Create, Replace, Update and Delete`_ draft specification, allowing
for transactional capabilities against feature and record data.

Furthermore, pygeoapi supports the `OGC API - Moving Features - Part 1: Core`_  international standard, allowing
for transactional capabilities against moving features.

To enable transactions in pygeoapi, a given resource provider needs to be editable (via the configuration resource provider
``editable: true`` property).  Note that the feature or record provider MUST support create/update/delete.  See the
:ref:`ogcapi-features` and :ref:`ogcapi-records` documentation for transaction support status of pygeoapi backends.
For MF-API transactions, please refer :ref:`ogcapi-mfapi`

Access control
^^^^^^^^^^^^^^

It should be made clear that authentication and authorization is beyond the responsibility of pygeoapi.  This means that
if a pygeoapi user enables transactions, they must provide access control explicitly via another service.

.. _`OGC API - Features - Part 4: Create, Replace, Update and Delete`: https://docs.ogc.org/DRAFTS/20-002.html
.. _`OGC API - Moving Features - Part 1: Core`: https://docs.ogc.org/is/22-003r3/22-003r3.html
