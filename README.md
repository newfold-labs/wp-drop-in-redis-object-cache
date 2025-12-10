<a href="https://newfold.com/" target="_blank">
    <img src="https://newfold.com/content/experience-fragments/newfold/site-header/master/_jcr_content/root/header/logo.coreimg.svg/1621395071423/newfold-digital.svg" alt="Newfold Logo" title="Newfold Digital" align="right" 
height="42" />
</a>

# WordPress Redis Object Cache Drop-In

[![Version Number](https://img.shields.io/github/v/release/newfold-labs/wp-drop-in-redis-object-cache?color=77dd77&labelColor=00000&style=for-the-badge)](https://github.com/newfold-labs/wp-drop-in-redis-object-cache/releases)

[![License](https://img.shields.io/github/license/newfold-labs/wp-drop-in-redis-object-cache?labelColor=333333&color=666666&style=for-the-badge)](https://raw.githubusercontent.com/newfold-labs/wp-drop-in-redis-object-cache/main/LICENSE)

A high-performance persistent object cache drop-in for WordPress powered by Redis. Integrated with Bluehost Plugin's Performance module for optimal performance.

## Overview

This drop-in provides a Redis-backed object cache for WordPress, replacing the default in-memory object cache with a persistent Redis implementation.

## Requirements

- WordPress 5.0+
- PHP 7.2+
- Redis server
- Bluehost Plugin with Performance module enabled (provides Predis library)

## Installation

1. Place `object-cache.php` in your WordPress `/wp-content/` directory
2. Ensure the Bluehost Plugin is installed with the Performance module in it
3. Configure Redis connection settings in `wp-config.php`

## Configuration

Add the following constants to your `wp-config.php` file:

```php
// Redis Object Cache Configuration
define( 'WP_REDIS_HOST', '127.0.0.1' );
define( 'WP_REDIS_PORT', 6379 );
define( 'WP_REDIS_DATABASE', 0 );
define( 'WP_REDIS_GRACEFUL', true );
```

See the [documentation](https://github.com/newfold-labs/wp-drop-in-redis-object-cache) for all available configuration options.

## License

GPL-2.0-or-later

