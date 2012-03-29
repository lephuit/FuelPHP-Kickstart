FuelPHP Bootstrap
-----------------
Preface this by saying that this is not an official FuelPHP application. FuelPHP Bootstrap is a maintained by me and used as a bootstrap for applications that I develop. I also use this as a
learning tool to try out new ideas that pop into my head from time to time.

Hopefully someone else will find this useful. Please do send me any feedback that you have. If you're curious as to why I've done something a certain way or if you have a better way of doing it,
please take a second to create an issue/pull request.

What's Included?
================
Initially this will be just a real simple bootstrap. We'll have migrations to get you up and running a complete system with sessions management (mysql backed), authentication using sentry, 
a common controller that you can extend to your other controllers, and a few other goodies.

I've chosen to include Twitter Bootstrap for design and assets simply because it is quick and simple. Once installed you can change that to anything you like!

Available Tasks:
================
I've included the following tasks to make your life a little easier. You may or may not need to run any or all of these tasks.  If you are using git, I do recommend running the "git" task
just to make sure certain files are ignored.

###Writable
use this if you are having issues with write permissions on your log, cache or config directories. This will set their permissions to 777.
	
	php oil r writable

###Git
This will do a simple "git update-index --assume-unchanged. This way you can upload to the repo with out these files being added, causing problems down the road and so you don't have
your DB password just hanging around in the web somewhere.
	
	php oil r git