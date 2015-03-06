---
title: Creting a simple console command  with laravel 5
layout: post
category: Linux
author: Eduardo Leiva
date: 2015-02-20
---
First

* php artisan list

next

* php artisan make:console FirstCommand --command=my:firstCommand

next

add your command on kernel file ( /app/Console/Kernel.php )


*	protected $commands = [
*		'App\Console\Commands\Inspire',
*		'App\Console\Commands\FirstCommand',
*	];

next

* php artisan list ( you will see your command )

next

comment this

  protected function getArguments()
	{
		return [
	//		['example', InputArgument::REQUIRED, 'An example argument.'],
		];
	}

next add this line

  public function fire()
	{
	    $this->info("Update Teams");
	}

next ready to go:

* php artisan my:firstCommand

:D
