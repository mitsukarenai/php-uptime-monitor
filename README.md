# PHP Uptime Monitor

> I've never thought of PHP as more than a simple tool to solve problems. -Rasmus Lerdorf

## What's that ?

PHP Uptime Monitor is a lightweight (yet dirty) PHP script that monitors external hosts or services. Basic sockets and cURL magic. Quick dirty HTML, butchered down eZ Server Monitor's CSS sheet, and a fucking JSON file as database because why the hell use a decent engine like SQLite, PGSQL or MariaDB, huh ? Why not a CouchDB or Cassandra, huh ? It's not like you gonna use that script for thousands of requests per second anyway *and it could still handle so much database parsing* so fuck it.
And oh: shameless including of two sounds, a crackhead .gitignore, an useless [license](LICENSE) file and this README. Ain't life sweet.

## Cut the crap. What can it do ?

- host check (TCP connection test)
- URL check (HTTP, HTTPS, FTP, SFTP). cURL can do more but.. oh let's keep it healthy for your mind

Of course since it's PHP, that's only gonna work per-script execution, soooo.. webcron or open tab in browser. 

## Screenshot !

Sure.

![logo](https://i.imgur.com/ZoHDeLD.png)

## Alright ! Huh.. how do I add servers to monitor ?

Edit the JSON. Manually.

## You're kidding me right ? This software is barely even complete..

Feel free to contribute, as-is it's good enough for my use, and I feel like I spent too much time coding this dirty pile of poop already :) Never intended to make a work of arts. (and too lazy to do a dirty auth system to allow an admin to easily manage monitors from web interface)

## But why didn't you simply use XXX or YYY ?

Nagios ? Hey, I want to monitor external systems, on shared hosting and whatnot. And stuff like Monitorus or Pingdom don't realtime monitor as free user, but hey paid plans are so insanely expensive.. I just want a quick head-up as soon a server doesn't respond correctly, there's no vital production systems running :(

## What's the database scheme ? How's the JSON handled ?

Take a look near end of the `index.php`. And there's comments all over the place :)

## Where do I set the notification email address ?

In the `db.json`

Have fun !
