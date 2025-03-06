# Modulo_Prestashop_Seur
Repositorio público del módulo oficial de SEUR para Prestashop

Changelog:

## [2.5.18] - 2025-02-27

### Added
- Add Update shipment feature
- Add packages feature

### Fixed
- Fix isPickupFrio
- Fix seur_url_basepath not initialized in one case
- Remove extra slash on AJAX URls


## [2.5.17] - 2025-02-03

### Added
- Add log info to UpdateShipmentStatus cron task
- Add another class selector to initSeurCarriers (pickup)
- Add all Seur COD manual payments if defined

### Fixed 
- Fix split error (pickup)
- Fix seurcashondelivery module value and seur_url_basepath value

## [2.5.16] - 2024-12-12

### Fixed

- Remove manual jQuery inclusion to prevent duplication in PrestaShop < 1.7.7
- Overwrite TCPDF Output function
- Save pickup address in Order and SeurOrder
- Cache selected pudoId at localStorage
- Relocation of pickup points
- Refactoring method getSeurProductType
- Improve pudo list

## [2.5.15] - 2024-10-30

### Fixed

- Multiples Seur2Shop configs
- Add extracondition to printMap
- Fix hook header return

## [2.5.14] - 2024-09-27

### Fixed

- Additional payments when SEUR2_SENDED_ORDER is active
- Select default pick-up point when google maps api fails
- JS/CSS scripts not enqueued on admin area

### Added

- Add option mark as shipped when generate manifest

## [2.5.13] - 2024-07-08

### Fixed

- Order_payment when no payments
- Url module ajax
- Total_shipping_tax_incl value
- COD logic in module


## [2.5.12] - 2024-05-16
Fixed
Deprecated OrderPayment::getByOrderId

Deprecated order shipping_number

Default value if no pickup is configured

Update ajax shipment url

‌

## [2.5.11] - 2024-04-16

‌

### Fixed

‌

Status update script URL
Seur carriers products and services urls when site is in subfolder
Set unused files as deprecated
‌

## [2.5.11] - 2024-04-16

‌

### Fixed

‌

Status update script URL
Seur carriers products and services urls when site is in subfolder
Set unused files as deprecated
‌

[2.5.10] - 2024-03-15
Added
Edit order product-service
Insured shipment option
GMap reload option and refactor
Change ISO:23412 condition
[2.5.9] - 2024-01-29
Fixed
Clean phone data
‌

[2.5.8] - 2024-01-16
Added
Add automatic package calculation
Add automatic creation labels
Changed
Delete class Town.php
Delete class Rate.php
Detete SOAP calls files
Delete deprecated merchant config fields
[2.5.7] -2023-11-14

### Added

Add PHP8 compatibility
Add platform name at shipment creation
### Changed

Adapt labels name file with "-"
### Fixed

Required pickup center selection
Fix lost invoice and delivery number
Fix lost id_carrier in cart
‌

[2.5.6] - 2023-04-21

### Added

Add Changelog
New cron script to update shipments status
Cron job as a CLI command
Page 'Seguimiento de envíos' reload timer
Return after error on processSingleShipment
Display a message on admin area on how to set up a scheduled task.
### Changed

Update status labels
Ignore cancel orders in status update
### Fixed

Fix shipping address when finally is not pickup
2.5.5 - 2023-03-20

Fix idNumber param in getExpedition
Fix PS 1.6 no vendor folder to tcpdf
Fix peso y bultos reset
Fix streetName max lenght
2.5.4 - 2023-02-08

Fix PDF merger
Add ISO info
Add A4_3 printer type
2.5.3 - 2023-01-19

Fix massive print
2.5.2 - 2023-01-13

Fix PDFMerger tcpdf library
2.5.1 - 2023-01-12

Fix massive print labels
Fix multiparcel print labels
Fix parcels and weigth reset in reprint
Fix file separator
2.5.0 - 2023-01-04

Add additional info in order comments
Add collection date in pickup
2.4.0 - 2022-12-14

Add products references in shipment comments
Config param: SEUR2_PRODS_REFS_IN_COMMENTS
2.3.10 - 2022-11-17

Fix shipping costs taxes with COD
Comment pod option in Label
actualizado tambiel el zip 2.3.9 (quitada url apipre)

2.3.9 - 2022-10-25

Fix tracking list url links
Fix International pickups
Pickups points - Show list if not Map API key
Fix fee note font size invoice pdf
Add service CLASSIC
Remove file label exists condition
Update invoice shipping totals with COD payment
Fix OnePageCheckout id_address_delivery
Fix manifest incidence codfee 0 value
API Migration expeditions and shipments
2.3.8 - 2022-07-18

Fix select shop multistore
2.3.7 - 2022-06-02

Sanitize & on customer data to label
Force registerHook
Fix no payments in order
Recalculate shipping cost with COD when order is edited in backend
2.3.6 - 2022-05-27

Fix F5 get print label
2.3.5 - 2022-05-17

Fix save label_file
Fix save order_weight
2.3.4 - 2022-04-28

Improve admin order templates
Add label_file field to store file name
2.3.3 - 2022-04-22

Fix url Labelary
Show Seur reference number
Fix Expeditions reference number
Multistore
2.3.2 - 2022-02-10

Migration International shippings (Geolabel, Brexit, Tariff)
Add params config label by reference/id
Add param config taric
Fix checkbox shippingAll
Fix operator ??
2.3.1 (beta) - 2021-11-19

Migration Pickups API REST
Migration PUDOs API REST
Fix catch order without invoice
Fix map points info
2.3.0 (beta) - 2021-10-28

Begin migration process to new API REST
2.2.2 - 2021-10-19

Fix Worten-Carrefour international shipping selection
Add saturday delivery on fridays
Fix refreshShippingCost in PS1.6
Fix Pdf headers in Manifest
2.2.1 - 2021-09-02

Fix type service select
Fix html encode in order messages
Change getExpeditions Soap call
Fix default ccc selection
2.2.0 - 2021-08-11

Improve tracking
Fix credentials label Geolabel
2.1.1.12 - 2021-06-15

Livetracking DPD
Fix order reference filter
Show error messages in create label function
2.1.1.11 - 2021-05-26

Automatize international shipping CCC selector
2.1.1.10 - 2021-05-20

Change payment CashOnDelivery when change order carrier to Seur
Fix js method to get id_order
2.1.1.9 - 2021-04-14

Fix CashOnDelivery value in manisfest
2.1.1.8 - 2021-04-12

Improve ecb update
Fix not hide last column on shipping order detail
Change Ireland post code to 1 when print label
2.1.1.7 - 2021-03-23

Fix order detail redirect and reference filter
Copy ecb and show in order list
2.1.1.6 - 2021-03-16

Fix Change ps_version to ps_version_seur
2.1.1.5 - 2021-03-11

Fix checkbox shippingAll
2.1.1.4 - 2021-02-18

Fix jquery load order on v1.7
