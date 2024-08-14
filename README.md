# Magento 2 Better IPs

A tiny little module to tell Magento to use different headers when determining the user's IP address.

The following headers will be checked in this order:
* `HTTP_CF_CONNECTING_IP`
* `HTTP_X_REAL_IP`
* `HTTP_X_FORWARDED_FOR`

By default, Magento then falls back to using the `REMOTE_ADDR` header.

---

To install:  
* `composer require webstraxt/m2-better-ips`
* `php bin/magento module:enable Webstraxt_BetterIPs`
* `php bin/magento setup:upgrade`

---

Copyright (C) 2024 Webstraxt Limited
