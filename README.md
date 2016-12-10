# İletiMerkezi-SMS Library for PHP

### Install

    composer require talhahavadar/iletimerkezi-sms

### For Laravel

First you need to install via composer after that you need to add `IletimerkeziSmsServiceProvider` to
`app/Providers/AppServiceProvider.php` file of your project.

    /**
     * Register any application services.
     *
     * @return void
     */
    public function register()
    {
        $this->app->register('IletimerkeziSms\IletimerkeziSmsServiceProvider');
    }
then you can run the command below:

    php artisan vendor:publish --tag=config

Then you need to enter your credentials to `config/iletimerkezi.php`
 file.

 You can find example usage of library in `tests/test.php` file.