# Archively
Simple collections management for small museums

## Features

- Cross-platform, works on Windows, Linux, and MacOS.
- 

## Getting Started

Download your binary.

When you open Archively for the first time, you'll be prompted to create a profile.

## Developers

### Data Format Requirement

This project is designed to work with data formatted according to the GraphletDB core schema. It is important that the data you use conforms to this schema to ensure proper functionality. For more information about the GraphletJS schema and how to structure your data accordingly, please refer to the [GraphletDB documentation](https://github.com/jennerhanni/GraphletDB/).

Archively defines a set of nodes which support Citation Style Language (CSL) fields to create bibliographies using CSL JSON or citeproc-js. 

### Archively Node Definitions

`archivelyapp.org/node/Item`

|Item||
|---|---|
|Vocabulary|http://archivelyapp.org/node|
|URI|http://archivelyapp.org/node/Item|
|Label|Item|
|Definition||
|Comment||
|Type of Term|Class|

|Property|Type|Default Value|Definition|
|---|---|---|---|
|radio__archivelyType|string|"Unassessed"|[link](http://archivelyapp.org/props/radio__archivelyType)|
|radio__dcmiType|string|""|[link](http://archivelyapp.org/props/radio__dcmiType)|
|radio__privacyStatus|string|"Unassessed"|[link](http://archivelyapp.org/props/radio__privacyStatus)|
|str__privacyReason|string|""|[link](http://archivelyapp.org/props/str__privacyReason)|
|bool__hasPhysicalObject|bool|false|[link](http://archivelyapp.org/props/bool__hasPhysicalObject)|
|str__internalNote|string|""|[link](http://archivelyapp.org/props/str__internalNote)|
|rel__items|list of id strings|[]|[link](http://archivelyapp.org/props/rel__items)|
|rel__containsItems|list of id strings|[]|[link](http://archivelyapp.org/props/rel__containsItems)|
|str__itemDescription|string|""|[link](http://archivelyapp.org/props/str__itemDescription)|
|rel__maker|list of id strings|[]|[link](http://archivelyapp.org/props/rel__maker)|
|rel__dateMade|list of id strings|[]|[link](http://archivelyapp.org/props/rel__dateMade)|
|str__productionNotes|string|""|[link](http://archivelyapp.org/props/str__productionNotes)|
|rel__placeMade|list of id strings|[]|[link](http://archivelyapp.org/props/rel__placeMade)|
|rel__mediumMaterials|list of id strings|[]|[link](http://archivelyapp.org/props/rel__mediumMaterials)|
|str__inscriptionMarks|string|""|[link](http://archivelyapp.org/props/str__inscriptionMarks)|
|str__language|string|""|[link](http://archivelyapp.org/props/str__language)|
|rel__keywords|list of id strings|[]|[link](http://archivelyapp.org/props/rel__keywords)|
|rel__acquisitionRecords|list of id strings|[]|[link](http://archivelyapp.org/props/rel__acquisitionRecords)|
|radio__physicalLocation|string|"Unassessed"|[link](http://archivelyapp.org/props/radio__physicalLocation)|
|str__specificLocation|string|""|[link](http://archivelyapp.org/props/str__specificLocation)|
|rel__controllingInstitution|list of id strings|[]|[link](http://archivelyapp.org/props/rel__controllingInstitution)|
|radio__rightsStatus|string|"Unassessed"|[link](http://archivelyapp.org/props/radio__rightsStatus)|
|str__rightsNote|string|""|[link](http://archivelyapp.org/props/str__rightsNote)|
|rel__childBinaryFiles|list of strings|[]|[link](http://archivelyapp.org/props/rel__childBinaryFiles)|

`archivelyapp.org/node/Keyword`

|Keyword||
|---|---|
|Vocabulary|http://archivelyapp.org/node|
|URI|http://archivelyapp.org/node/Keyword|
|Label|Keyword|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/node/List`

|List||
|---|---|
|Vocabulary|http://archivelyapp.org/node|
|URI|http://archivelyapp.org/node/List|
|Label|List|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/node/User`

|User||
|---|---|
|Vocabulary|http://archivelyapp.org/node|
|URI|http://archivelyapp.org/node/User|
|Label|User|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/node/ItemAcquisition`

|ItemAcquisition||
|---|---|
|Vocabulary|http://archivelyapp.org/node|
|URI|http://archivelyapp.org/node/ItemAcquisition|
|Label|ItemAcquisition|
|Definition||
|Comment||
|Type of Term|Class|

### Archively Property Definitions

`archivelyapp.org/props/radio__archivelyType`

|radio__archivelyType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/radio__archivelyType|
|Label|radio__archivelyType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/radio__dcmiType`

|radio__dcmiType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/radio__dcmiType|
|Label|radio__dcmiType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/radio__privacyStatus`

|radio__privacyStatus||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/radio__privacyStatus|
|Label|radio__privacyStatus|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__privacyReason`

|str__privacyReason||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__privacyReason|
|Label|str__privacyReason|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/bool__hasPhysicalObject`

|bool__hasPhysicalObject||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/bool__hasPhysicalObject|
|Label|bool__hasPhysicalObject|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__internalNote`

|str__internalNote||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__internalNote|
|Label|str__internalNote|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__items`

|rel__items||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__items|
|Label|rel__items|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__containsItems`

|rel__containsItems||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__containsItems|
|Label|rel__containsItems|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__containedByItems`

|rel__containedByItems||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__containedByItems|
|Label|rel__containedByItems|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__itemDescription`

|str__itemDescription||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__itemDescription|
|Label|str__itemDescription|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__maker`

|rel__maker||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__maker|
|Label|rel__maker|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__dateMade`

|rel__dateMade||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__dateMade|
|Label|rel__dateMade|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__productionNotes`

|str__productionNotes||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__productionNotes|
|Label|str__productionNotes|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__placeMade`

|rel__placeMade||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__placeMade|
|Label|rel__placeMade|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__mediumMaterials`

|rel__mediumMaterials||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__mediumMaterials|
|Label|rel__mediumMaterials|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__inscriptionMarks`

|str__inscriptionMarks||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__inscriptionMarks|
|Label|str__inscriptionMarks|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__language`

|str__language||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__language|
|Label|str__language|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__keywords`

|rel__keywords||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__keywords|
|Label|rel__keywords|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__acquisitionRecords`

|rel__acquisitionRecords||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__acquisitionRecords|
|Label|rel__acquisitionRecords|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/radio__physicalLocation`

|radio__physicalLocation||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/radio__physicalLocation|
|Label|radio__physicalLocation|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__specificLocation`

|str__specificLocation||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__specificLocation|
|Label|str__specificLocation|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__controllingInstitution`

|rel__controllingInstitution||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__controllingInstitution|
|Label|rel__controllingInstitution|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/radio__rightsStatus`

|radio__rightsStatus||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/radio__rightsStatus|
|Label|radio__rightsStatus|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__rightsNote`

|str__rightsNote||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__rightsNote|
|Label|str__rightsNote|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__childBinaryFiles`

|rel__childBinaryFiles||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__childBinaryFiles|
|Label|rel__childBinaryFiles|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/radio__keywordType`

|radio__keywordType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/radio__keywordType|
|Label|radio__keywordType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__description`

|str__description||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__description|
|Label|str__description|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__users`

|rel__users||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__users|
|Label|rel__users|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__slug`

|str__slug||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__slug|
|Label|str__slug|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__lists`

|rel__lists||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__lists|
|Label|rel__lists|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/radio__recordType`

|radio__recordType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/radio__recordType|
|Label|radio__recordType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__associatedItem`

|rel__associatedItem||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__associatedItem|
|Label|rel__associatedItem|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__provenanceDetails`

|str__provenanceDetails||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__provenanceDetails|
|Label|str__provenanceDetails|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__provenancePlace`

|str__provenancePlace||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__provenancePlace|
|Label|str__provenancePlace|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__provenanceEntity`

|rel__provenanceEntity||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__provenanceEntity|
|Label|rel__provenanceEntity|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__price`

|str__price||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__price|
|Label|str__price|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__condition`

|str__condition||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__condition|
|Label|str__condition|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__date`

|str__date||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__date|
|Label|str__date|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__fileExt`

|str__fileExt||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__fileExt|
|Label|str__fileExt|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__localFilePath`

|str__localFilePath||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__localFilePath|
|Label|str__localFilePath|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__fileSize`

|str__fileSize||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__fileSize|
|Label|str__fileSize|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__numPdfPages`

|str__numPdfPages||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__numPdfPages|
|Label|str__numPdfPages|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__parentItem`

|rel__parentItem||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__parentItem|
|Label|rel__parentItem|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/radio__cslType`

|radio__cslType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/radio__cslType|
|Label|radio__cslType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslTitle`

|str__cslTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslTitle|
|Label|str__cslTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslAbstractNote`

|str__cslAbstractNote||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslAbstractNote|
|Label|str__cslAbstractNote|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__cslArtworkMedium`

|rel__cslArtworkMedium||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__cslArtworkMedium|
|Label|rel__cslArtworkMedium|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslArtworkSize`

|str__cslArtworkSize||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslArtworkSize|
|Label|str__cslArtworkSize|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__cslDate`

|rel__cslDate||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__cslDate|
|Label|rel__cslDate|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslLanguage`

|str__cslLanguage||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslLanguage|
|Label|str__cslLanguage|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslShortTitle`

|str__cslShortTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslShortTitle|
|Label|str__cslShortTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslArchive`

|str__cslArchive||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslArchive|
|Label|str__cslArchive|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslArchiveLocation`

|str__cslArchiveLocation||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslArchiveLocation|
|Label|str__cslArchiveLocation|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslLibraryCatalog`

|str__cslLibraryCatalog||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslLibraryCatalog|
|Label|str__cslLibraryCatalog|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCallNumber`

|str__cslCallNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCallNumber|
|Label|str__cslCallNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslUrl`

|str__cslUrl||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslUrl|
|Label|str__cslUrl|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslAccessDate`

|str__cslAccessDate||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslAccessDate|
|Label|str__cslAccessDate|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslRights`

|str__cslRights||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslRights|
|Label|str__cslRights|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslExtra`

|str__cslExtra||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslExtra|
|Label|str__cslExtra|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__cslCreator`

|rel__cslCreator||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__cslCreator|
|Label|rel__cslCreator|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__cslAudioRecordingFormat`

|rel__cslAudioRecordingFormat||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__cslAudioRecordingFormat|
|Label|rel__cslAudioRecordingFormat|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslSeriesTitle`

|str__cslSeriesTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslSeriesTitle|
|Label|str__cslSeriesTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslVolume`

|str__cslVolume||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslVolume|
|Label|str__cslVolume|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslNumberOfVolumes`

|str__cslNumberOfVolumes||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslNumberOfVolumes|
|Label|str__cslNumberOfVolumes|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslPlace`

|str__cslPlace||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslPlace|
|Label|str__cslPlace|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslLabel`

|str__cslLabel||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslLabel|
|Label|str__cslLabel|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslRunningTime`

|str__cslRunningTime||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslRunningTime|
|Label|str__cslRunningTime|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslISBN`

|str__cslISBN||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslISBN|
|Label|str__cslISBN|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslBillNumber`

|str__cslBillNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslBillNumber|
|Label|str__cslBillNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCode`

|str__cslCode||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCode|
|Label|str__cslCode|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCodeVolume`

|str__cslCodeVolume||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCodeVolume|
|Label|str__cslCodeVolume|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslSection`

|str__cslSection||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslSection|
|Label|str__cslSection|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCodePages`

|str__cslCodePages||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCodePages|
|Label|str__cslCodePages|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslLegislativeBody`

|str__cslLegislativeBody||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslLegislativeBody|
|Label|str__cslLegislativeBody|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslSession`

|str__cslSession||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslSession|
|Label|str__cslSession|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslHistory`

|str__cslHistory||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslHistory|
|Label|str__cslHistory|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslBlogTitle`

|str__cslBlogTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslBlogTitle|
|Label|str__cslBlogTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslWebsiteType`

|str__cslWebsiteType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslWebsiteType|
|Label|str__cslWebsiteType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslSeries`

|str__cslSeries||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslSeries|
|Label|str__cslSeries|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslSeriesNumber`

|str__cslSeriesNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslSeriesNumber|
|Label|str__cslSeriesNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslEdition`

|str__cslEdition||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslEdition|
|Label|str__cslEdition|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslPublisher`

|str__cslPublisher||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslPublisher|
|Label|str__cslPublisher|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslNumPages`

|str__cslNumPages||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslNumPages|
|Label|str__cslNumPages|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslBookTitle`

|str__cslBookTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslBookTitle|
|Label|str__cslBookTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslPages`

|str__cslPages||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslPages|
|Label|str__cslPages|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCaseName`

|str__cslCaseName||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCaseName|
|Label|str__cslCaseName|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCourt`

|str__cslCourt||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCourt|
|Label|str__cslCourt|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslDateDecided`

|str__cslDateDecided||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslDateDecided|
|Label|str__cslDateDecided|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslDocketNumber`

|str__cslDocketNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslDocketNumber|
|Label|str__cslDocketNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslReporter`

|str__cslReporter||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslReporter|
|Label|str__cslReporter|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslReporterVolume`

|str__cslReporterVolume||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslReporterVolume|
|Label|str__cslReporterVolume|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslFirstPage`

|str__cslFirstPage||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslFirstPage|
|Label|str__cslFirstPage|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslVersionNumber`

|str__cslVersionNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslVersionNumber|
|Label|str__cslVersionNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslSystem`

|str__cslSystem||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslSystem|
|Label|str__cslSystem|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCompany`

|str__cslCompany||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCompany|
|Label|str__cslCompany|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslProgrammingLanguage`

|str__cslProgrammingLanguage||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslProgrammingLanguage|
|Label|str__cslProgrammingLanguage|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslProceedingsTitle`

|str__cslProceedingsTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslProceedingsTitle|
|Label|str__cslProceedingsTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslConferenceName`

|str__cslConferenceName||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslConferenceName|
|Label|str__cslConferenceName|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslDOI`

|str__cslDOI||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslDOI|
|Label|str__cslDOI|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslDictionaryTitle`

|str__cslDictionaryTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslDictionaryTitle|
|Label|str__cslDictionaryTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslSubject`

|str__cslSubject||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslSubject|
|Label|str__cslSubject|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslEncyclopediaTitle`

|str__cslEncyclopediaTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslEncyclopediaTitle|
|Label|str__cslEncyclopediaTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslDistributor`

|str__cslDistributor||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslDistributor|
|Label|str__cslDistributor|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslGenre`

|str__cslGenre||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslGenre|
|Label|str__cslGenre|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslVideoRecordingFormat`

|str__cslVideoRecordingFormat||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslVideoRecordingFormat|
|Label|str__cslVideoRecordingFormat|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslForumTitle`

|str__cslForumTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslForumTitle|
|Label|str__cslForumTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslPostType`

|str__cslPostType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslPostType|
|Label|str__cslPostType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCommittee`

|str__cslCommittee||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCommittee|
|Label|str__cslCommittee|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslDocumentNumber`

|str__cslDocumentNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslDocumentNumber|
|Label|str__cslDocumentNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/rel__cslInterviewMedium`

|rel__cslInterviewMedium||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/rel__cslInterviewMedium|
|Label|rel__cslInterviewMedium|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslPublicationTitle`

|str__cslPublicationTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslPublicationTitle|
|Label|str__cslPublicationTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslIssue`

|str__cslIssue||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslIssue|
|Label|str__cslIssue|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslSeriesText`

|str__cslSeriesText||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslSeriesText|
|Label|str__cslSeriesText|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslJournalAbbreviation`

|str__cslJournalAbbreviation||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslJournalAbbreviation|
|Label|str__cslJournalAbbreviation|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslISSN`

|str__cslISSN||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslISSN|
|Label|str__cslISSN|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslLetterType`

|str__cslLetterType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslLetterType|
|Label|str__cslLetterType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslManuscriptType`

|str__cslManuscriptType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslManuscriptType|
|Label|str__cslManuscriptType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslMapType`

|str__cslMapType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslMapType|
|Label|str__cslMapType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslScale`

|str__cslScale||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslScale|
|Label|str__cslScale|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCountry`

|str__cslCountry||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCountry|
|Label|str__cslCountry|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslAssignee`

|str__cslAssignee||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslAssignee|
|Label|str__cslAssignee|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslIssuingAuthority`

|str__cslIssuingAuthority||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslIssuingAuthority|
|Label|str__cslIssuingAuthority|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslPatentNumber`

|str__cslPatentNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslPatentNumber|
|Label|str__cslPatentNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslFilingDate`

|str__cslFilingDate||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslFilingDate|
|Label|str__cslFilingDate|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslApplicationNumber`

|str__cslApplicationNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslApplicationNumber|
|Label|str__cslApplicationNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslPriorityNumbers`

|str__cslPriorityNumbers||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslPriorityNumbers|
|Label|str__cslPriorityNumbers|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslIssueDate`

|str__cslIssueDate||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslIssueDate|
|Label|str__cslIssueDate|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslReferences`

|str__cslReferences||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslReferences|
|Label|str__cslReferences|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslLegalStatus`

|str__cslLegalStatus||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslLegalStatus|
|Label|str__cslLegalStatus|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslEpisodeNumber`

|str__cslEpisodeNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslEpisodeNumber|
|Label|str__cslEpisodeNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslAudioFileType`

|str__cslAudioFileType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslAudioFileType|
|Label|str__cslAudioFileType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslPresentationType`

|str__cslPresentationType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslPresentationType|
|Label|str__cslPresentationType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslMeetingName`

|str__cslMeetingName||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslMeetingName|
|Label|str__cslMeetingName|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslProgramTitle`

|str__cslProgramTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslProgramTitle|
|Label|str__cslProgramTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslAudioRecordingFormat`

|str__cslAudioRecordingFormat||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslAudioRecordingFormat|
|Label|str__cslAudioRecordingFormat|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslNetwork`

|str__cslNetwork||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslNetwork|
|Label|str__cslNetwork|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslReportNumber`

|str__cslReportNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslReportNumber|
|Label|str__cslReportNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslReportType`

|str__cslReportType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslReportType|
|Label|str__cslReportType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslInstitution`

|str__cslInstitution||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslInstitution|
|Label|str__cslInstitution|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslNameOfAct`

|str__cslNameOfAct||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslNameOfAct|
|Label|str__cslNameOfAct|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCodeNumber`

|str__cslCodeNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCodeNumber|
|Label|str__cslCodeNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslPublicLawNumber`

|str__cslPublicLawNumber||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslPublicLawNumber|
|Label|str__cslPublicLawNumber|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslDateEnacted`

|str__cslDateEnacted||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslDateEnacted|
|Label|str__cslDateEnacted|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslThesisType`

|str__cslThesisType||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslThesisType|
|Label|str__cslThesisType|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslUniversity`

|str__cslUniversity||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslUniversity|
|Label|str__cslUniversity|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslStudio`

|str__cslStudio||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslStudio|
|Label|str__cslStudio|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslWebsiteTitle`

|str__cslWebsiteTitle||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslWebsiteTitle|
|Label|str__cslWebsiteTitle|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslRepository`

|str__cslRepository||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslRepository|
|Label|str__cslRepository|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslArchiveID`

|str__cslArchiveID||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslArchiveID|
|Label|str__cslArchiveID|
|Definition||
|Comment||
|Type of Term|Class|

`archivelyapp.org/props/str__cslCitationKey`

|str__cslCitationKey||
|---|---|
|Vocabulary|http://archivelyapp.org/props|
|URI|http://archivelyapp.org/props/str__cslCitationKey|
|Label|str__cslCitationKey|
|Definition||
|Comment||
|Type of Term|Class|
