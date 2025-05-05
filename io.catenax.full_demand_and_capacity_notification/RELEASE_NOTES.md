# Changelog
All notable changes to this model will be documented in this file.

## [3.0.0] - 2025-0x-yz

### Added

- added field resolvingMeasureDescription
- created composure

### Changed

- sourceNotificationId: 
  - renamed to sourceNotificationId and elaborated semantics
  - now is mandatory
- relatedNotificationId: 
  - changed to be a collection (relatedNotificationIds)
  - added logic when a notification can be considered a related notification - TODO: do we need to also consider things that may affect materials that are an input of he current material? What do I do with a relatedNotificationId if I don't have additional information? Do I need to consider also multiple sourceDisruptionIds?
- leadingRootCauseEnumeration: added thirdPartyMisplanning, insolvency
- Introduce a Set of Material Entities with materialNumberCustomer, materialNumberSupplier and materialGlobalAssetId
 - materialNumberSupplier and materialNumberCustomer use the PartIdCharacterstic from PartTypeInformation
 - materialNumberSupplier is mandatory
 - materialGlobalAssetId uses the UUID characteristic directly


### Removed
