## Note:
This is just like Creolab/Image, I just want to rename the alias so it doesn't overlap the Intervention/Image one.

Image
=====

Resize, crop and cache images for Laravel 4.
Framework agnostic coming soon.

## Installation

Simply add the following to your **composer.json** file:

    "lostcause/image": "dev-master"

And you can also add the service provider to **app/config/app.php**:

    'Creolab\Image\ImageServiceProvider',

And register the facade in the same file under aliases:

    'CreolabImage' => 'Creolab\Image\ImageFacade',

## Usage

You can use the library directly in your views like this:

    <img src="{{ CreolabImage::resize('public/path/to/image.jpg', 640, 480) }}">

Also to generate square thumbs:

    <img src="{{ CreolabImage::thumb('public/path/to/image.jpg', 80) }}">

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/creolab/image/trend.png)](https://bitdeli.com/free "Bitdeli Badge")
