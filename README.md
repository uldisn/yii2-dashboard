# Yii2 Dashboard

[![Yii2](https://img.shields.io/badge/Powered_by-Yii_Framework-green.svg?style=flat)](https://www.yiiframework.com/)
[![Latest Version](https://img.shields.io/github/tag/cornernote/yii2-dashboard.svg?style=flat-square&label=release)](https://github.com/cornernote/yii2-dashboard/tags)
[![Software License](https://img.shields.io/badge/license-BSD-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Coverage Status](https://img.shields.io/scrutinizer/coverage/g/cornernote/yii2-dashboard.svg?style=flat-square)](https://scrutinizer-ci.com/g/cornernote/yii2-dashboard/code-structure)
[![Quality Score](https://img.shields.io/scrutinizer/g/cornernote/yii2-dashboard.svg?style=flat-square)](https://scrutinizer-ci.com/g/cornernote/yii2-dashboard)
[![Total Downloads](https://img.shields.io/packagist/dt/cornernote/yii2-dashboard.svg?style=flat-square)](https://packagist.org/packages/cornernote/yii2-dashboard)
[![Yii2 Framework](https://img.shields.io/badge/extension-Yii2_Framework-green.svg?style=flat-square)](http://www.yiiframework.com/extension/yii2-dashboard)

Yii2 Dashboard is a module that allows you to create and manage dashboards using custom layouts and panels.


## Features

* Create custom [layouts](http://cornernote.github.io/yii2-dashboard/docs/layouts/) with regions where panels can be placed.
* Create custom [panels](http://cornernote.github.io/yii2-dashboard/docs/panels/) to display your data inside a layout region.
* Drag-and-drop interface to rearrange panels inside a layout.


## Documentation

Getting started? Try the [Installation Guide](https://cornernote.github.io/yii2-dashboard/docs/installation/).  You will find further information in the [Documentation](https://cornernote.github.io/yii2-dashboard/docs/).

For changes since the last version see the [Changelog](https://github.com/cornernote/yii2-dashboard/blob/master/CHANGELOG.md).

## Config

```php
<?php
$config = [
    'modules' => [
        'dashboard' => [
            'class' => 'cornernote\dashboard\Module',
            'layouts' => [
                'default' => 'cornernote\dashboard\layouts\DefaultLayout',
                'example' => 'tests\app\dashboard\layouts\ExampleLayout',
            ],
			'updateRoles' => ['dashboardAdmin'],
            'panels' => [
                'example' => [
					'class' => 'app\dashboard\panels\ExamplePanel',
					'allowRules => ['exampleRule'],	
				],
            ],
            'dashboards' => [
                'dashboard first' => [
					'viewRoles => ['firstRule'],	
				],
            ],
        ],
    ],
];
```


## Screenshots

![Dashboard View](https://cloud.githubusercontent.com/assets/51875/8636670/21febed6-28ae-11e5-8fc7-dc57e5bbc422.png)

More images are available from the [Screenshots](https://cornernote.github.io/yii2-dashboard/screenshots/) page.


## Contributing

Contributions are welcome.  Please refer to the [contributing guidelines](CONTRIBUTING.md).

Thanks to [everyone who has contributed](CREDITS.md).


## Project Resources

* [Project Homepage](https://cornernote.github.io/yii2-dashboard)
* [Live Demo](http://yii2-dashboard.herokuapp.com/)
* [GitHub Project](https://github.com/cornernote/yii2-dashboard)
* [Yii2 Extension](http://www.yiiframework.com/extension/yii2-dashboard)
* [Packagist Package](https://packagist.org/packages/cornernote/yii2-dashboard)
* [Travis CI Testing](https://travis-ci.org/cornernote/yii2-dashboard)
* [Scrutinizer CI Code Quality](https://scrutinizer-ci.com/g/cornernote/yii2-dashboard)


## License

BSD-3 - Please refer to the [license](LICENSE.md).
