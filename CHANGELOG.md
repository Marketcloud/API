# CHANGELOG

## 0.17.30
* Fixed validation of `category` GET parameter in `GET /v0/products` endpoint. Now correctly validating it, requiring a string data type.
* Fixed Model definition for Coupons resource: property `usages_left` is now required to be >= 0
* Fixed coupons validation, now correctly requiring a target_id for types `PRODUCT_COUPON` and `CATEGORY_COUPON`
* Fixed sub-resource validation now correctly returning the index of the invalid sub-resource
