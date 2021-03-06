# Chance

[![Chance Logo](http://chancejs.com/logo.png)](http://chancejs.com)

[![Build Status](https://travis-ci.org/victorquinn/chancejs.png)](https://travis-ci.org/victorquinn/chancejs)

Chance - Random generator helper for JavaScript

Homepage: [http://chancejs.com](http://chancejs.com)

Many more details on [http://chancejs.com](http://chancejs.com) but this single
library can generate random numbers, characters, strings, names, addresses,
dice, and pretty much anything else.

It includes the basic building blocks for all these items and is built on top
of a Mersenne Twister so it can generate these things with repeatability, if
desired.

## Packages

### Bower

It can also be used with [Bower](http://bower.io)

```
bower install chance
```

then in the HTML of your app:
<!--this is just here to force an update-->
```html
<!-- Load Chance -->
<script type="text/javascript" src="app/bower_components/chance/chance.min.js"></script>
<script>
    // Use Chance immediately!
    alert(chance.string());
</script>
```

### Component

It can also be used with [Component](http://component.io)

```
component install victorquinn/chancejs
```

then in the HTML of your app:

```html
<!-- Load Chance -->
<script type="text/javascript" src="components/victorquinn-chancejs/chance.js"></script>
<script>
    // Use Chance immediately!
    alert(chance.string());
</script>

### npm

```shell
npm install chance
```

### spm [![](http://spmjs.io/badge/chance)](http://spmjs.io/package/chance)

It can also be used with [spm](http://spmjs.io/package/chance).

```
spm install chance
```

## Usage

### Browser

Chance instantiates itself onto the window. This means that in the simplest case you can just include the script tag then use an instance of Chance immediately.

```html
<script src="chance.js"></script>
<script>
    console.log(chance.string());
</script>
```

[More info](http://chancejs.com#browser)

### CLI

To use Chance from the command line, install it globally with:

```shell
npm install -g chance
```

Then invoke any generator by name, like so:

```shell
$ chance name --prefix
Dr. Georgia Sanchez

$ chance latitude --min 12.34 --max 56.78
22.01836
```

### Node.js

And it can be used in Node.js.

```js
var Chance = require('chance'),
    chance = new Chance();

// Get a random zip code
chance.zip();
```

### RequireJS

Chance also includes an AMD define so it can be used with RequireJS.

```js
require(['Chance'], function(Chance) {
    // Instantiate
    var chance = new Chance();
       
    // Then just use it:
    var my_random_integer = chance.integer();
});
```

## Author
### Victor Quinn
[http://victorquinn.com](http://victorquinn.com)

Please feel free to reach out to me if you have any questions or suggestions.

### Contributors

THANK YOU!

```
 project  : chancejs
 repo age : 1 year, 7 months
 active   : 120 days
 commits  : 447
 files    : 24
 authors  :
   305	Victor Quinn        68.2%
    26	Oliver Salzburg     5.8%
    13	Tim Petricola       2.9%
    12	Alex DiLiberto      2.7%
    11	davmillar           2.5%
     7	Jan Tojnar          1.6%
     5	Michael Cordingley  1.1%
     5	Matt Klaber         1.1%
     4	Chris Villarreal    0.9%
     4	Abhijeet Pawar      0.9%
     4	Avishaan            0.9%
     4	Kevin Garnett       0.9%
     3	Nicholas Johnson    0.7%
     3	qjcg                0.7%
     3	Alexandr Lozovyuk   0.7%
     3	Dominic Barnes      0.7%
     2	xshyamx             0.4%
     2	Adam Krebs          0.4%
     2	Andreas Koeberle    0.4%
     2	Iskren Chernev      0.4%
     2	Nathan MacInnes     0.4%
     2	Pascal Borreli      0.4%
     2	SeeSchloss          0.4%
     2	Stefan Penner       0.4%
     2	dhilipsiva          0.4%
     2	path411             0.4%
     2	shyam               0.4%
     1	Richard Anaya       0.2%
     1	afc163              0.2%
     1	Johannes Stein      0.2%
     1	ddunning            0.2%
     1	Doug Lawrence       0.2%
     1	flrent              0.2%
     1	kkroner             0.2%
     1	leesei              0.2%
     1	Ryan Tenney         0.2%
     1	Samuel Greene       0.2%
     1	lkptrzk             0.2%
     1	Brian.Barnett       0.2%
     1	Ng Patrick          0.2%
```

### Contribute! 

Be a part of this project! You can run the test using the following.
1. Install dependencies from package.json by running `npm install`
2. Install dependencies for testing by running `bower install`
3. Run the test via `npm test`
4. Make some fun new modules!

This project is licensed under the [MIT License](http://en.wikipedia.org/wiki/MIT_License) so feel free to hack away :)

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/victorquinn/chancejs/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

Proudly written in Washington, D.C.

