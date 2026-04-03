<a href="https://newfold.com/" target="_blank">
    <img src="https://newfold.com/content/experience-fragments/newfold/site-header/master/_jcr_content/root/header/logo.coreimg.svg/1621395071423/newfold-digital.svg" alt="Newfold Logo" title="Newfold Digital" align="right" 
height="42" />
</a>

# WordPress Redis Object Cache Drop-In

A persistent object cache drop-in for WordPress powered by Redis. Replaces the default in-memory object cache with a Redis-backed implementation for improved performance across page loads.

## Features

- Supports PhpRedis, Predis, and Credis client libraries
- Redis Cluster, Sentinel, Replication, and Sharding support
- Selective flush via key prefix (`WP_REDIS_PREFIX`)
- Per-group flush and unflushable groups
- Batch operations (`add_multiple`, `set_multiple`, `get_multiple`, `delete_multiple`)
- Optional igbinary serialization
- Graceful fallback to in-memory cache on connection failure

## Requirements

- WordPress 5.0+
- PHP 7.2+
- Redis server
- A supported Redis client library (PhpRedis extension, Predis, or Credis)

## Installation

Place `object-cache.php` in your WordPress `wp-content/` directory.

## License

GPL-3.0-or-later
