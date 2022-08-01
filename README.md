# A PHP project skeleton

based on https://github.com/koriym/Koriym.PhpSkeleton

## Create Project

To create your project, enter the following command in your console.

```
composer create-project shotanue/php-skeleton <project-path>
```

## dependencies

* [PHPUnit](https://phpunit.readthedocs.io/ja/latest/)
* [PHP_CodeSniffer](https://github.com/squizlabs/PHP_CodeSniffer/wiki)
* [Psalm](https://psalm.dev)
* [PHPMetrics](https://www.phpmetrics.org)
* [Rector](https://www.phpmetrics.org)


## debug skeleton

```
mkdir build

cd build

cat << EOF > package.json
{
    "package": {
        "name": "shotanue/php-skeleton",
        "version": "0.0.0",
        "source": {
            "url": "./../.git",
            "type": "git",
            "reference": "main"
        }
    }
}
EOF

composer create-project --repository-url=./package.json shotanue/php-skeleton test
```
