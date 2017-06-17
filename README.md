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

in case you don't have [bower](TBD) installed globally.

Finally, simply start the service

```
$npm start
```

and modify the component. The browser will be reloaded dynamically as you modify code.

## How it works

The project simply make use of [browser-sync](TBD).

The actual command line used is the following:

```
$ browser-sync start --server app -f app --serveStatic bower_components --no-notify
```

* The command expects your code / project to be sitting in the `app` folder. Change as desired
* `bower_components` files will be served synamically, which means you don't need to reference the `bower_components folder when using external dependencies`.
 

## Author

* Julien Lengrand-Lambert <@jlengrand>

## LICENSE

See LICENSE file