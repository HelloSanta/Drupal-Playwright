# Drupal Playwright Docker Image

Docker image for running Drupal with Playwright testing capabilities.

## Features

- PHP 8.3 with Apache
- All required PHP extensions for Drupal
- Node.js 20 (LTS)
- Playwright dependencies for Chromium browser
- MySQL client and rsync for database operations

## Usage

```dockerfile
FROM hellosanta/drupal-playwright:8.3

# Add your Drupal files
COPY . /var/www/html
```

## Available Tags

- `8.4` - PHP 8.4 with Playwright support
- `8.3` - PHP 8.3 with Playwright support

## Building Locally

```bash
docker build -t hellosanta/drupal-playwright:8.3 -f 8.3/Dockerfile .
```

## Related Projects

- [Drupal-Cypress](https://github.com/hellosanta/Drupal-Cypress) - Cypress version of this image
