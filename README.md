# Webflow Script Conditional Loader

This project includes a dynamic script loader that determines which script to load based on the current environment and domain. The loader is designed to be flexible and easily configurable for different deployment scenarios.

## Overview

The loader script is written in JavaScript and is embedded within an HTML file. It dynamically sets the source of a script element based on the hostname of the current window location. This allows for different scripts to be loaded in development, QA, and production environments.

## Features

- **Environment Detection**: The script can detect whether it is running in a QA or production environment.
- **Domain-Based Script Loading**: Different scripts can be loaded based on the domain name.
- **Deferred Script Loading**: The script element is created with the `defer` attribute to ensure it does not block the initial page load.

## Configuration

### QA Flag

The `isQAReady` variable is a boolean flag that determines whether the QA script should be loaded. Set this to `true` to load the production script in all environments.
