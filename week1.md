* implicit conversion is called coercion
`console.log(3+'4') = "34" `
`console.log('3'+4) = "34" ` 
`console.log('3'*'4') = 12 ` 

* let follows block scope

* var does not follow block scope

* `let x=1;
{
	var x=2;
	console.log(`x is : ${x}`);
}
console.log(x is : ${x});`

  - the code gives error :
  - "<a class='gotoLine' href='#45:0'>45:0</a> SyntaxError: Cannot declare a var variable that shadows a let/const/class variable: 'x'."

* `var x=1;
{
	let x=2;
	console.log(x is : ${x});
}
console.log(x is : ${x});`

  - output :
  - "x is : 2"
  - "x is : 1"

* IIFE => (function () {return "hello" }() ) => declare and invoke

* Regular function declaration
`function add(x, y)
{
  return x + y;
}`
 
* Named variable declaration
`let add = function(x, y)
{
  return x + y;
}`

* Arrow function declaration
`let add = (x, y) => x + y;`

* this gives Reference Error
`{
	let x=5;
}
console.log(x);
`

* All are valid function definitions
  - `const sum = (x, y) => {return x+y}`
  - `const sum = (x, y) => x+y`
  - `const sqr = x => {return x*x}`
  - `const sqr = x => x*x`
