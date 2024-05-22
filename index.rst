################################################################
Rules of Engagement for Accessing Data During the Embargo Period
################################################################


.. abstract::

   Data must be embargoed after arriving at the USDF - for 30 days in commissioning and 80 hrs in Survey Operations. Alert Processing will not record vetoed streaks. What rules will we impose on accessing data during that period?

Embargo Restrictions
====================

Embargoed data types cannot leave the USDF during the embargo period.
LSST Users, such as those who have been granted USDF accounts via the Resource Allocation Process, will not have access to the data in the embargo rack.
Rubin Observatory staff (including the Commissioning Team) will have full access to the data in the embargo rack as their Rubin roles require. 
(Some Rubin roles require only LSST User permissions). 
Any data can reside transiently on batch or kubernetes processing nodes but must be deleted after use.

Access to the embargo rack will be enforced with permissions.

All user-generated data products derived from the embargo repo should be written back to the embargo repo.  While catalogs can theoretically be exported, it is simpler to just keep everything there.

Exempted Data types
===================

Derived calibrations, which are not generated from sky pixels, can be exported from the embargo repo as needed.

Post-Embargo
============

Selected datasets, including both raw and prompt-processed, will be copied from the embargo rack/repo to normal storage and ingested into staff and public Butler repos once the embargo period is over.  User-generated datasets can be copied as well at this time if arrangements are made to include them in the configuration.  Those datasets that are to be released will be made available to the US DAC to be viewed by anyone with data rights.  Raw images will be registered in Rucio for transmission to FrDF and UKDF.

Removal from the embargo repo can occur after a successful copy to normal storage, or it can be postponed for a configurable time period, but space limitations mean that no dataset should be expected to be retained for more than 30 days in the embargo repo.

Handling of the Satellite Catalog
=================================

The catalog will be treated as CUI Basic, per DOE Order 471.7. As such, access will be restricted to authorized individuals, identified in an approved acccess list and allowed access to the catalog via permissions set on a directory in the embargo rack filesystem. 
The catalogs may not leave that directory, except for transient copies needed by prompt/alert processing. 
No derivative catalogs may be stored.
