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
    
<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
