---
title: Web UI
---


# Chronos Web UI

### Compiling Assets

**Node.js is required to build assets**

Assets are automatically compiled when running `mvn package`. If you change assets, and want them updated in your jar, you must either `rm -rf src/main/resources/assets/build` or `mvn clean`.

### Modifying Assets

To modify assets and have changes reflected on the fly, you will need to start Chronos with a specially configured YAML file. The configuration is quite simple and is documented at [dropwizard-configurable-assets-bundle](https://github.com/bazaarvoice/dropwizard-configurable-assets-bundle/blob/master/README.md).

There are also two included example YAML files that make use of this configuration:

* [config/local_scheduler.yml](/mesos/chronos/blob/master/config/local_scheduler.yml#L4)
* [config/local_scheduler_nozk.yml](/mesos/chronos/blob/master/config/local_scheduler_nozk.yml#L7)

### Build Requirements

When building and optimizing the assets, make sure you have at least 1GB of RAM available.