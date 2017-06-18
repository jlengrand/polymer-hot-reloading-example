# A simple example of Polymer project with hot reloading

## To test it

```
$ npm install
```

and then

```
$ bower install
```

or 

```
$ ./node_modules/.bin/bower install
```

in case you don't have [bower](https://bower.io/) installed globally.

Finally, simply start the service

```
$npm start
```

and modify the component. The browser will be reloaded dynamically as you modify code.

## How it works

The project simply make use of [browser-sync](https://browsersync.io/).

The actual command line used is the following:

```
$ browser-sync start --server app -f app --serveStatic bower_components --no-notify
```

* The command expects your code / project to be sitting in the `app` folder. Change as desired
* `bower_components` files will be served synamically, which means you don't need to reference the `bower_components folder when using external dependencies`.

Your browser should open a new tab by itself once browser sync is running. Otherwise, navigate to [http://localhost:3000](http://localhost:3000). 

Also, think about checking out [http://localhost:3001/](http://localhost:3001/) for the browsersync overview. 

## Author

* Julien Lengrand-Lambert <@jlengrand>

## LICENSE

See LICENSE file