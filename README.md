# Minimal Magento 2 Open Source

A stripped-down, high-performance Magento 2 installation optimized for speed and essential e-commerce functionality. This project removes bloated modules and third-party tools to deliver a lightweight, blazing-fast open-source e-commerce platform.

I managed to install and use this Magento on a shared hosting plan for €5/month.

**What you will not have:**

- ElasticSearch / OpenSearch
- MSI
- GraphQL
- RabbitMQ
- Page Builder
- 2FA
- Google, PayPal, Adobe, Fedex, DHL, UPS, Vertex, AWS, Klarna, Dotmailer, Amazon, New Relic...

## Current Version

Official Magento OpenSource 2.4.8-p3

## Installation

### Clone repository

```bash
git clone https://github.com/magentix/minimal-magento-open-source.git magento
```

```bash
cd magento
```

### Eliminate the repository dependency

```bash
rm -rf .git
```

### Install Magento

```bash
composer install
```

### Setup database

```bash
bin/magento setup:install \
--base-url="http://localhost.magento/" \
--db-host="localhost" \
--db-name="magento" \
--db-user="root" \
--db-password="xxx" \
--admin-firstname="John" \
--admin-lastname="Doe" \
--admin-email="john@example.com" \
--admin-user="john" \
--admin-password="xxx" \
--language="en_US" \
--currency="USD" \
--use-rewrites="1" \
--backend-frontname="admin"
```
