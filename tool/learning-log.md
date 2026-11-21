# Tool Learning Log

## Tool: **Math and Typescript**

## Project: **Make #1 -- > #2 using math.**

---
### Week 1
* Had difficulties getting math js to work at all. Ended up copy and pasting script source from [here](https://jsbin.com/devacu/edit?html,output)
* Learned to use math.evaluate()
1. Uses lower case 'math' unlike actual java where you need uppercase. Ex. `Math.ceil()`
2. Takes in an expression and returns output. The input has to be a string or array which doesn't make a lot of sense but oh well.
* Made a simple function that finds if prompted expression equals the number one.
``` js
    function equal_one(num){
        return num == 1
    }
    var expression = prompt("Type an expression you believe to be equal to one!")
    document.write(equal_one(math.evaluate(expression)))
```
## Week 2 + 3
* Tried out math.chain() where it allowed you to chain math symbols after one another by following up math.chain with `.add(num)`,`.subtract(num)`, etc. Used the exaple on the website example to help me. [Here](https://mathjs.org/).
    * Example:
    ``` js
    math.chain(3) // 3 is start
    .add(5) // add 5
    .multiple(8) // multiple by 8
    .divide(2) // divide by 2
    .done() // Finish the chain, Not needed just reminder.
    ```
* Tested out math.evaluate()'s ability to use imaginary numbers. Although very similair to normal sqrt, `Math.sqrt(4) //2` , it can now return imaginary numbers aswell. `math.sqrt(-4) // 2i`. (All that is changed is a lowercase 'm' in 'math'.)
    * Using booleans, I compared the 2i to a normal number like 2 out of curiosity.
    ``` js
    if(math.sqrt(-4) > 2){
        document.write("yes")
    }else if(math.sqrt(-4) < 2){
        document.write("no")
     }else{
         document.write("maybe") // It returned maybe.
    }
    ```
## Week 4
* Learn how to use 'scope()' via looking at examples of other bigger topics (scope was uesd on the side). Assigns values to variables that can be called upon in later equations
    * Ex.
    ``` js
    var scope = {
        a: 3,
        b: 4
    }
    math.evaluate('a+b',scope) //7
    ```
* In the example, I had to specify which scope I used because you can have a differnt values for the same variable if you make multiple scopes. An example is seem below of two scopes being used:
    * Ex.
    ``` js
    var scope = {
        a: 3,
        b: 4
    }
    var scope2 = {
        a: 5,
        b: 10
    }
    math.evaluate('a+b',scope2) // Now will be 15
    ```
    This can probably be used for figuring which set of numbers you want to use for this problem even if the variables are the same.
* You can also change a value of a variable like that of a list. For a list, you would do: `lst[0] = "new value"`. On the otherhand, for a scope, you would place the variable name of the scope, following by a '.' then the vairable you wish to change equal to its new value. Ex:
    * 
    ``` js 
    var scope = {
        a: 5
    }
    scope.a = 8
    math.evaluate('a*a',scope) // 64 instead of 25
<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
