---
What is difference between module.exports and export?:

The module is a plain JavaScript object with an exports property. Exports is a plain JavaScript variable that happens to be set to module.exports. At the end of your file, node.js will basically ‘return’ module.exports to the require function. A simplified way to view a JS file in Node could be this:

var module = { exports: {} };
var exports = module.exports;

// your code
return module.exports;

If you set a property on exports, like exports.a = 9;, that will set module.exports.a as well because objects are passed around as references in JavaScript, which means that if you set multiple variables to the same object, they are all the same object; so then exports and module.exports are the same objects.
But if you set exports to something new, it will no longer be set to module.exports, so exports and module.exports are no longer the same objects.
-----------------------------------
Dot (.) Operator

The dot is used in Javascript to break up objects. 

Property accessors provide access to an object's properties by using the dot notation or the bracket notation.

Ex:
----

var person = {};
person['firstname'] = 'Mario';
person['lastname'] = 'Rossi';

console.log(person.firstname);
// expected output: "Mario"

person = {'firstname': 'John', 'lastname': 'Doe'}

console.log(person['lastname']);
// expected output: "Doe"
-----------------------------------


