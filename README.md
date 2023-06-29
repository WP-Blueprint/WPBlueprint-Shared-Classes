# WP Blueprint Theme Core

WP Blueprint Theme Core is a versatile framework that serves as a solid foundation for WordPress Themes, providing essential reusable functionalities and a streamlined development workflow to enhance efficiency, flexibility, and compatibility.

## Features

- Object-Oriented Programming (OOP) structure for better organization and extensibility.
- Shared functionalities for WordPress themes.
- Reusable classes for settings, security, enqueuing, Gutenberg, navigation, options, post types, taxonomies, widget areas, patterns, and shortcodes.

## Requirements

- **PHP:** This theme requires PHP 5.6 or higher.
- **WordPress:** A WordPress installation of 5.6 or higher is required.
- **Composer:** The theme is installable via Composer from Packagist, but can also be manually downloaded and installed.

## Installation

To install the WP Blueprint Theme Core as a dependency in your project, use Composer:

```shell
composer require wp-blueprint/theme-core
```

## Usage

After installing the WP Blueprint Theme Core, you can utilize the `Initializer` class to load and register the shared classes in your theme:

```php
if ( class_exists( 'WPBlueprint\\Theme\Core\Initializer' ) ) :
	WPBlueprint\Theme\Core\Initializer::register_services();
endif;
```

## Backlog

Here are some features and improvements planned for future releases:

- **Finish development and thorough testing:** Ensure its functionality, performance, and compatibility with various browsers and devices.

## Development

[![Code Quality - WPCS](https://github.com/WP-Blueprint/wp-blueprint-theme-core/actions/workflows/lint-wpcs.yml/badge.svg)](https://github.com/WP-Blueprint/wp-blueprint-theme-core/actions/workflows/lint-wpcs.yml) [![Code Quality - PHP](https://github.com/WP-Blueprint/wp-blueprint-theme-core/actions/workflows/lint-php.yml/badge.svg)](https://github.com/WP-Blueprint/wp-blueprint-theme-core/actions/workflows/lint-php.yml)

Use the following scripts to aid in development:

- `composer run lint:wpcs`: WPCS Lint
- `composer run lint:wpcs:fix`: WPCS Fix
- `composer run lint:php`: PHP Lint

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to help improve this project.

Please follow the [WordPress Coding Standards](https://developer.wordpress.org/coding-standards/wordpress-coding-standards/) and ensure that your changes are well-documented. Use the provided npm scripts for linting your PHP code before submitting.

## License

This project is licensed under the [GNU General Public License v3.0](https://www.gnu.org/licenses/gpl-3.0).
