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
<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
