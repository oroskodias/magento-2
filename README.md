# Order Created Webhooks of Magento 2 for fomo.com

![Preview](https://github.com/usefomo/magento-2/blob/master/.github/admin.png?raw=true)

This module provides webhooks for Magento 2 events, specially for fomo.com

> Currently guaranteed for Magento 2 GA.

We're hopeful the community can help push this effort forward through this module.

## Getting Started

Upload to folder (you may need to create subfolders)
```
app/code/Fomo/Webhook
```

Add `Fomo_Webhook` to your `app/etc/config.php`
```php
<?php
return array (
  'modules' => 
  array (
    //
    // Bunch of other modules
    // 
    'Fomo_Webhook' => 1,
  ),
);
```

Run database migrations
```
php bin/magento setup:upgrade
```

## Supported Webhooks

Available now
- Order created.

## Play Loads

- first_name
- last_name
- email
- city
- province
- country
- subtotal
- grandtotal
- payment_method
- product["id"]
- product["price"]
- product["type"]
- product["qty"]
- product["price"]


## Contributing

Submit a pull request!
