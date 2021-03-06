# PHP Cleaner library (DEPRECATED)

[![Latest Stable Version](https://poser.pugx.org/josantonius/cleaner/v/stable)](https://packagist.org/packages/josantonius/cleaner) [![Total Downloads](https://poser.pugx.org/josantonius/cleaner/downloads)](https://packagist.org/packages/josantonius/cleaner) [![Latest Unstable Version](https://poser.pugx.org/josantonius/cleaner/v/unstable)](https://packagist.org/packages/josantonius/cleaner) [![License](https://poser.pugx.org/josantonius/cleaner/license)](https://packagist.org/packages/josantonius/cleaner)

[Versión en español](README-ES.md)

PHP class for cleaning resources.

---

- [Installation](#installation)
- [Requirements](#requirements)
- [Quick Start and Examples](#quick-start-and-examples)
- [Available Methods](#available-methods)
- [Usage](#usage)
- [Tests](#tests)
- [Contribute](#contribute)
- [Repository](#repository)
- [License](#license)
- [Copyright](#copyright)

---

### Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

To install PHP Cleaner library, simply:

    $ composer require Josantonius/Cleaner

The previous command will only install the necessary files, if you prefer to download the entire source code (including tests, vendor folder, exceptions not used, docs...) you can use:

    $ composer require Josantonius/Cleaner --prefer-source

Or you can also clone the complete repository with Git:

	$ git clone https://github.com/Josantonius/PHP-Cleaner.git

### Requirements

This library is supported by PHP versions 5.6 or higher and is compatible with HHVM versions 3.0 or higher.

### Quick Start and Examples

To use this class, simply:

```php
require __DIR__ . '/vendor/autoload.php';

use Josantonius\Cleaner\Cleaner;
```
### Available Methods

Available methods in this library:

```php
Cleaner::unregisterGlobals();
Cleaner::stripSlashesDeep();
Cleaner::removeMagicQuotes();
```
### Usage

Example of use for this library:

```php
<?php
require __DIR__ . '/vendor/autoload.php';

use Josantonius\Cleaner\Cleaner;

Cleaner::removeMagicQuotes();
Cleaner::unregisterGlobals();
```

### Tests 

To use the [test](tests) class, simply:

```php
<?php
$loader = require __DIR__ . '/vendor/autoload.php';

$loader->addPsr4('Josantonius\\Cleaner\\Tests\\', __DIR__ . '/vendor/josantonius/cleaner/tests');

use Josantonius\Cleaner\Tests\CleanerTest;

```
Available test methods in this library:

```php
CleanerTest::testRemoveMagicQuotes();
CleanerTest::testUnregisterGlobals();
```

### Contribute
1. Check for open issues or open a new issue to start a discussion around a bug or feature.
1. Fork the repository on GitHub to start making your changes.
1. Write one or more tests for the new feature or that expose the bug.
1. Make code changes to implement the feature or fix the bug.
1. Send a pull request to get your changes merged and published.

This is intended for large and long-lived objects.

### Repository

All files in this repository were created and uploaded automatically with [Reposgit Creator](https://github.com/Josantonius/BASH-Reposgit).

### License

This project is licensed under **MIT license**. See the [LICENSE](LICENSE) file for more info.

### Copyright

2017 Josantonius, [josantonius.com](https://josantonius.com/)

If you find it useful, let me know :wink:

You can contact me on [Twitter](https://twitter.com/Josantonius) or through my [email](mailto:hello@josantonius.com).