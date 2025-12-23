# Minimal Magento 2 Open Source

A stripped-down, high-performance Magento 2 installation optimized for speed and essential e-commerce functionality. This project removes bloated modules and third-party tools to deliver a lightweight, blazing-fast open-source e-commerce platform.

## Overview

**Minimal Magento 2** is a curated Magento 2 distribution that retains only the core e-commerce features you need while eliminating unnecessary modules and external commercial integrations. The result is a significantly faster, leaner platform perfect for merchants who want maximum performance with minimal overhead.

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

### Remove repository dependence

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
