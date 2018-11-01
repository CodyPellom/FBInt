JavaScript Concepts to Master 
*_*_*_*_*_*_*_*_*_*_*_*_*_*_*_*_*_*

Data types: 
*Undefined
*Null
*Boolean
*String
*Symbol
*Number
*Object
-----------------------------------
JavaScript was invented in 1995 and was first used by the netscape browser
-----------------------------------
What are Arrow Functions? 
()=>{}

Arrow functions are a concise and short way to write finction expressions in Es6 and above. A row function cannot be used as constructors and also does not support the '.this' argument, super or new.target keywords. 

Ex: 
 const greet=()=>{console.log('hello');}
 greet();
-----------------------------------
Importing and Exporting 

The purpose of importing and exporting files in JavaScript is the ability to split code up into multiple files. Importing and exporting is also used for grabbing bits of code from JS libraries. 

Ex:
 //index.js

 import name,age from './person'; 

 console.log(name);
 console.log(age);

 //person.js

 let name ='Sharad', occupation='developer', age =26;

 export { name, age};
 ---------------------------------

