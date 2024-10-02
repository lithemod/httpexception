# Lithe HttpException

Custom HTTP exceptions for the Lithe.

## Installation

You can install this package via [Composer](https://getcomposer.org/). Follow the instructions below:

### Step 1: Add the package

Run the following command to add the package to your project:

```bash
composer require lithemod/httpexception
```

### Step 2: Autoloading

The package uses the PSR-4 autoloading standard. The exceptions will be available under the `Lithe\Exceptions\Http` namespace. Make sure that autoloading is properly configured in your project.

### Step 3: Usage

You can now use the custom HTTP exceptions in your project. Example usage:

```php
use Lithe\Exceptions\Http\HttpException;

try {
    throw new HttpException(404, 'Page not found');
} catch (HttpException $e) {
    echo 'Error ' . $e->getStatusCode() . ': ' . $e->getMessage();
}
```

## License

This package is licensed under the MIT license. See the [LICENSE](LICENSE) file for more details.