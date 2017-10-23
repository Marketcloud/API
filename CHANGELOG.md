# CHANGELOG

## 0.17.34
* Fixed items_total calculations, now `price_discount` can be equal to zero to achieve "free" products.
* Fixed internal method for calculating `payment_method_total`

## 0.17.33
* Performance improvements for 2 core middlewares.
* Added support new notification type, emitted when a new invoice is created.

## 0.17.32
* Improved products model validation by enforcing consistency of `stock_type` `stock_level` and `stock_status`

## 0.17.31
* Enhanced behaviour of `category` GET parameter in `GET /v0/products` endpoint. Now allowing a comma separated list of paths as input and returning products matching at least one of those category paths.

## 0.17.30
* Fixed validation of `category` GET parameter in `GET /v0/products` endpoint. Now correctly validating it, requiring a string data type.
* Fixed Model definition for Coupons resource: property `usages_left` is now required to be >= 0
* Fixed coupons validation, now correctly requiring a target_id for types `PRODUCT_COUPON` and `CATEGORY_COUPON`
* Fixed sub-resource validation now correctly returning the index of the invalid sub-resource
