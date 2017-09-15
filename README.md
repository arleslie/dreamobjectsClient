# arleslie\DreamObjects
Client for DreamObjects to work with AWS S3 API (for Laravel)

# Installation
`composer require arleslie/dreamobjects-client`

In `config\filesystems.php` add the following under `'disks' => [`
```
        'dreamobjects' => [
            'driver' => 'dreamobjects',
            'key'    => env('DREAMO_KEY'),
            'secret' => env('DREAMO_SECRET'),
            'bucket' => env('DREAMO_BUCKET'),
            'host' => env('DREAMO_HOST', 'http://objects.dreamhost.com')
        ],
```

Add the ServiceProvider: `arleslie\DreamObjects\ServiceProvider` to your `app.php`.
