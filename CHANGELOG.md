# Change Log
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## 2.0.5
  - Fixes #408 Correct Subdivision files for AD, AE, AF, AG, and AL

## 2.0.4
  - Update cache.

## 2.0.3
  - Fix comparison with country to nil
  - Add NANP_prefix as separate field

## 2.0.2
  - Add nanp_prefix data.

## 2.0.1
- Content updates
  - Fix bounding boxes that were mismatched.
- Update bounding box update task to prevent any lookup from return anything other than a country.

## 2.0.0
- Remove find_country_by_translations

## 2.0.0.rc3
- Content updates
  - All geo cords, are no longer strings
  - All bounding boxes updated
  - United States is now United States of America
- Refactor of Rake tasks

## 2.0.0.rc2
- Add fallback when looking up locales for pt-BR style languages
- Implement project style guide

## 2.0.0.rc
- Fixed a regression that would purge the countries memory cache when adding a custom country #353
- Various Content Updates

## 2.0.0.pre.4
- Fix crash when app introduces an unexpected locale. Much thanks to @jstenhouse

## 2.0.0.pre.2
- Bringing in content from 1.x branch

## 2.0.0.pre
- Selective loading translations of countries
- Auto detect I18n locales to load
- Add Configuration methods to force locales to load
- Dropped currencies gem in favor of money
- Add Time Zone Support
- DATA STRUCTURE CHANGES
  -COUNTRY
    - BREAKING CHANGES
      - names: => unofficial_names
      - languages: => official_languages
      - lat/lng fields are nested under a "geo" key
    - + spoken_languages
    - +


## 1.2.5 @ 2016-01-22
- Rebuilding cache

## 1.2.4 @ 2016-01-21
- Romanian Standard VAT rate is 20% as of 2016-01-01 #325 @dougal
- Palestine submit #324 @samizan
- Added 47 as calling code for Bouvet Island, Norwegian territory #323
- Added XAF as currency code for Congo @espen
- Force converting passed locale to string @borodiychuk

## 1.2.3
- Content Updates

## 1.2.2
- Content Updates

## 1.2.1
- Fixed issue in loading @rposborne

## 1.2.0 (yanked)
- Cleaning up Global Load Path @rposborne
- Add MOP as the currency for Macao @kriskhaira

## 1.1.0
- Adding compare operation to country @guilleart
- Content Updates @rposbone
- Correct NL to NO for un_locode @ohenrik
- Fix spelling of Sjælland @boatrite
- Add alternate spelling of Macao/Macau @nityaoberoi

## 1.0.0
- Switch to Marshalling for cache storage @rposborne
- Country class helper now must be explicitly loaded @rposborne
- Removed Rails 2.0 FormHelper COUNTRIES @rposborne
- Add class codes method to get list of all alpha2 codes @rposborne
- Change default behavior of all method to return a list of country objects vs a tuple of alpha code + name

## 0.11.5
- Refactored data loading into it's own class
- Added ability to override bad translations from i18n
- Update languages in NO.yml @matfiz
- Fix Subdivisions & States in README @pnomolos
- Fix New York, Washington, Oklahoma state's latitude/longitude information @GUI
- Bad state data present in Uruguay has been removed @saisha92
- Various Other Content Updates by @danshultz @embs @sykaeh, @tg0

## 0.11.4
- Added coordinates for subdivisions @fabn
- Various Other Content Updates by @fabn, @snowblink

## 0.11.3
- Translations update from i18n-data

## 0.11.2
- silence ruby warnings @franckverrot
- add find_country_by_translated_name @rposborne NOTE: this is garbage for the
  time being, some translations have duplicates in them and causes false results

## 0.11.1
- added bounding box coordinates for VI, CW, PR, AS, and GU : @marinom
- revert Lookup country by translated name via find_by_name @rposborne

## [0.11.0] - 2015-03-03
### Changed
- Cached Translations in gem to translation lookup speed @rposborne, @stayhero
- Upgrade test suite to rspec 3 @rposborne
- Added region_short for postal codes @stayhero
- Content Updates @masolino, @rosetree, @stayhero, @skarlcf, @cllns, @speric, @rposborne
- Adding Lat/Lng to countries @jabawack81
- Readme Updates @cllns
