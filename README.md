# Drupal-check Docksal Addon

## Installation

Download or clone the drupal-check addon and place it into your .docksal/addons directory.

```shell
cd .docksal/addons
git clone https://github.com/cbarrettgenuine/drupal-check.git
fin addon install drupal-check
```

## Usage

This tool works on all Drupal code.

### 2. Run drupal-check

Usage:

  ```shell
  fin drupal-check [MODULE NAME] [OPTIONS]
  ```

Arguments:

* `MODULE NAME` - The modules machine name.
* `OPTIONS` - See "Options" for allowed values.

Options:

* `-a` Check analysis
* `-d` Check deprecations (default)
* `-t` Module type {core, custom, contrib (default)}

Examples:

* Check the address contrib module:

  ```shell
  drupal-check address
  ```

* Check non-contrib module:

  ```shell
  drupal-check custom_module -t custom
  ```

* Check the address contrib module for deprecations:

  ```shell
  drupal-check address -d
  ```

* Check the address contrib module for analysis:

  ```shell
  drupal-check address -a
  ```