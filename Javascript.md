### Variable
- let -> if you plan to reassign
- const -> not reassigning
- var -> function scope, legacy code, no error if you reinitialize. /// function{var=10,const=5{var=11,const=6}->var=11,const5}
- `Hey ${myVar}` -> Hey Arnold
- Scope: local > function > global

### See result
- console.log()

### Browser javascript
- alert()
- confirm() -> Ok===True // Cancel===False
- prompt() -> Enter Text here: Ok === True // Cancel===False
- location.reload()

### Data types
- string
- number
- boolean
- undefined
- null
- ,
- string + number = turns number to string

### Operations
- +
- -
- *
- /
- %
- myVar = myVar + 1
- myVar += 1
- myVar++

### Operations Boolean
- ===
- !==
- <=
- >=
- .
- &&
- ||
- .
- myVar -> if myVar is true
- !myVar -> if myVar is false
- myVar ?? -> has a value (accepts "")

###  Variable info
- typeof
- .length

### String Methods
> Mathematics
- .charAt(0) -> "M"
- .indexOf("at") -> 1
- .lastIndexOf("at") -> 6
- .slice(5, 8) -> "mat" /// slice(5) -> matics
- .toUpperCase() -> "MATHEMATICS"
- .toLowerCase() -> "mathematics"
- .includes("mat") -> true
- .split("e") -> ["Math", "matics"] /// .split("") -> ["M", "a", "t", "h", "e", "m", "a", "t", "i", "c", "s"] /// .split(" "//",")
- "Hey      ".trim() -> "Hey"

## Number Methods
- 42.0 === 42 // 42.1 !== 42
- Number("425") -> 425 /// Number("Hi"//undefined) -> NaN /// Number(true//false) -> 1//0
- Number.isInteger(43.5) -> false
- Number.parseFloat("42.123abc") -> 42.123
- Number.parseInt("42.123abc") -> 42
- 45.04059.toFixed(2) -> "45.04"
- 45.6492.toString() -> "45.6492"
- Number.isNaN("Hey") -> false /// isNaN("Hey) -> true

### Math method
- Math.PI -> 3.141592653589793
- Math.trunc(3.999) -> 3
- Math.round(3.5) -> 4
- Math.ceil(3.001) -> 4
- Math.floor(3.999) -> 3
- Math.pow(5, 3) -> 125
- Math.min(2.4,5,9,2) -> 2
- Math.max(2,5,9,9.4) -> 9.5
- Math.random() -> 0-0.9999 /// Math.floor(Math.random()*10)+1 -> 1-10


## Conditionals

#### if else
- if (condition) {action}
- else if (condition) {action}
	- if (condition) {action}
- else {action}

#### switch
- switch (expression OR value -> myVar // 5 // "hey") {
	- case 1:
		- action;
		- break;
	- case "bla":
		- action;
		- break;
	- default:
		- action;
- }

#### Ternary
- condition ? ifTrue : ifFalse;
- condition ? ifTrue : condition ? ifTrue : ifFalse;



## Loops

#### while
- while (condition) {action}

#### do while
- do {action}
- while (condition)
- -> does it at least one time, even if condition false

#### for
- for (let i = 0; i < 10; i++) { action }
- for (let i = 0; i < myArr.length; i++) { action[i] }
- let i = 0; for (; i < 10;) {action; i++;}

#### Loop actions
- break; -> gets out of loop when it reaches break
- continue; -> when it reaches continue, continue loop back at top or beginning, skip bottom of continue


## Functions

- function sum() {return 2+2;} // sum() -> 4
- function sum(x,y) {return x+y;} // sum(1,2) -> 3
- const sum = function (x,y) {return x+y;} // sum(4,5) -> 9
- const sum = (x,y) => {return x+y;} // sum(2,3) -> 5


## Arrays
> [a,b,c,d,e]
- myArray[0] = "Hey" -> Adds "Hey" in position 0 (works with const)
- .length /// [myArray.length-1]
- .push("Hey") -> Adds "Hey" to end -> [a,b,c,d,e,"Hey"]
- .pop() -> Removes last item -> [a,b,c,d]
- .unshift(42) -> Adds 42 to start [42,a,b,c,d,e]
- .shift() -> Removes first item -> [b,c,d,e]
- delete myArray[1] -> leaves[1] as undefined, doesnt erase -> [a,undef,c,d,e]
- .splice(1,2,42) // [1,2,3,4] -> [1,42,4] /// .splice(position,numReplaced,replaceWith) -> [a,42,d,e]
- .slice(1,4) -> [b,c,d]
- .reverse() -> [e,d,c,b,a]
- .join() // ["a","b","c"] -> a,b,c
- .split(",") // "A,B,C" -> ["A","B","C"]
- .concat() // ["d","e"].concat["a","b"] -> ["d","e","a","b"]
- [...arrB, ...arrA] // ["d","e"] ["a","b"] -> ["d","e","a","b"]
- myArr[2][1][5][3] -> to access nested arrays, just add more

## Objects
- myObj.name_id === myObj[name_id]

### Regex
- \n => Skip to next line