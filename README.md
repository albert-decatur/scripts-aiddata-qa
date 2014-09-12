scripts-aiddata-qa
==================

Scripts for AidData quality assessment.
These are largely generic and can apply to any TSV.
The purposes of the scripts are to:

* working with Geonames
  * pull geonames fields from their API by geonameid
  * check that geonames feature type and precision code combos follow user supplied rules
* check cardinality of fields
  * is the relationship one-to-one?
  * are pairs of values unique?
* date handling
  * find invalid dates, including invalid leap days
  * convert to ISO 8601 (YYYY-MM-DD)
* deflation
  * make GDP deflators
  * apply GDP deflators
  * check for null values in deflator outputs
* handling nulls
  * find percent of records that are null, by field
* duplicates
  * find which fields contribute the most to records being non-duplicates

Prerequisites:

* mawk
* GNU parallel

TODO
====

Script to pull from Geonames txt dump.
