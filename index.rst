################################################################
Rules of Engagement for Accessing Data During the Embargo Period
################################################################


.. abstract::

Data must be embargoed after arriving at the USDF - for 30 days in
Commissioning prior to System First Light, and 80 hours thereafter.  What rules will we impose on accessing data during that period?

Embargo Restrictions
====================

Embargoed data types containing pixels are stored in the embargo rack during the embargo period.
LSST Users, including those who have been granted USDF accounts for "User Batch" processing via the Resource Allocation Process, will not have access to the data in the embargo rack.
Rubin Observatory staff (including the Commissioning Team) will have full access to the data in the embargo rack as their Rubin roles require. 
(Some Rubin roles require only LSST User permissions). 
Limited amounts of Embargoed data can reside transiently outside the embargo rack on batch or Kubernetes processing nodes or personal/work laptops/desktops or USDF home/shared/scratch directories but must be deleted after use.

Access to the embargo rack will be enforced via control of the relevant read credentials.

All user-generated data products derived from the embargo repo should be written back to the embargo repo.  While catalogs can theoretically be exported, it is simpler to just keep everything there.

Exempted Data types
===================

Derived calibrations, which are not generated from sky pixels, can be exported from the embargo rack as needed.

Post-Embargo
============

Selected datasets, including both raw and prompt-processed, will be copied from the embargo rack/repo to normal storage and ingested into staff and public Butler repos once the embargo period is over.  User-generated datasets can be copied as well at this time if arrangements are made to include them in the configuration.  Those datasets that are to be released will be made available to the US DAC to be viewed by anyone with data rights.  Raw images will be registered in Rucio for transmission to FrDF and UKDF.

Removal from the embargo repo can occur after a successful copy to normal storage, or it can be postponed for a configurable time period, but space limitations mean that no dataset should be expected to be retained for more than 30 days in the embargo repo.

Handling of the Satellite Catalog
=================================

The catalog and the credentials to retrieve new versions of it, as per DOE Order 471.7, will be restricted to authorized individuals, identified in an approved access list.
The catalog will reside in the memory of the Satellite Catalog Service and will not be persisted to non-volatile storage.
The access credentials will be encrypted at rest at all times.
No derivative catalogs will be stored.
