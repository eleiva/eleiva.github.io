---
title: Creting a simple console command  with laravel 5
layout: post
category: Linux
author: Eduardo Leiva
date: 2015-02-20
---

#### See your list of commands ( All that laravel has )
```
$ php artisan list
```
#### Create your command template:
```
$ php artisan make:console FirstCommand --command=my:firstCommand

```
#### Tell laravel about your new command: ( /app/Console/Kernel.php )
```php
*	protected $commands = [
*		'App\Console\Commands\Inspire',
*		'App\Console\Commands\FirstCommand',
*	];
```
#### Check if your commmand exist:
```
$ php artisan list 
```
#### You have to comment this ( next go back here )
```
  protected function getArguments()
	{
		return [
	//		['example', InputArgument::REQUIRED, 'An example argument.'],
		];
	}
```
### Add some text on out :
```
  public function fire()
	{
	    $this->info("Update Teams");
	}
```
## Run your great command:
```
$ php artisan my:firstCommand
```
:D
