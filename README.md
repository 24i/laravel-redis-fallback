# Redis cache fallback for Laravel 5

If you use Redis as cache driver on Laravel 5 and for some reason Redis server became unavailable, you will end up with a Connection Refused exception.
This package simply checks for the connection and if test fails, cache is switched to file driver.
As soon as Redis come back it will be used again.