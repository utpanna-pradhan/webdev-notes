# --------------------------------------------HR QNA-----------------------------------------------------
# 1. Tell me about yourself .

# 2. Why should we hire you instead of others?

# 3. Tell me about a time you failed in a project.

# 4. Tell me about one mistake you made in a project and how you handled it.
During my internship i was instructed to complete a task with a deadline.But i could estimate it too early and gave an early deadline, which lead to incomplition of task .So from that experience i got to know that i have to estimate task more time than it actually required ,so when i complete it before time it'll boost my confidence.

# 5. Where do you see yourself in the next 3 years?
As i have interst in GenAI i can see my self in a product based company where i can use my fullstack technology and integrate AI with it and make a large scalable product that will have millions of user.

# 6. Tell me about a time when you faced pressure to meet a deadline. How did you handle it?

# 7. If you are assigned a task you don’t know, what steps would you take?
First of all i will note down everything i need to complete.Then i will ask all possible questions to complete the task and a reference to it.I will ask chatgpt to summaries the task and ask reference.I divide the task into smaller sections and start by doing simple task at first then i will move to complicated one.



# -----------------------------------------------TECHNICAL QNA-------------------------------------------


# 4. What are semantic HTML tags? Why do we use them?
"Semantic HTML tags clearly describe the purpose of the content to both the browser and developers. Examples include <header>, <footer>, <main>, <section>, <article>, and <nav>. While they don’t change the visual result directly, they improve accessibility for screen readers, help search engines understand the page structure, and make code more readable."

# 5. Difference between inline, block, and inline-block elements?
"Inline elements (like <span>, <a>, <img>) only take up as much width as their content and don’t start on a new line. Block elements (like <div>, <p>, <h1>–<h6>) take the full width of the container and always start on a new line. Inline-block elements behave like inline elements but allow you to set width and height, which normal inline elements don’t support."

# 6. How does CSS specificity work? Explain with an example.
"CSS specificity determines which style will be applied when multiple rules target the same element. The priority is: Inline styles (highest) > ID selectors > Class/attribute/pseudo-class selectors > Element/pseudo-element selectors (lowest). If two rules have the same specificity, the one written later in the stylesheet takes priority."

Example:
```html
#title { color: red; }   /* ID → higher priority */
.title { color: blue; }  /* Class → lower priority */
h1 { color: green; }     /* Element → lowest priority */

```
Here, #title wins.

# 7. What are media queries? Why are they important in responsive design?
"Media queries are a feature in CSS that allow us to apply different styles depending on conditions such as screen width, height, or device orientation. They are essential for responsive design because they help ensure a website looks good and functions well on desktops, tablets, and mobile devices."

# 10. (Bonus) Explain the difference between relative, absolute, and fixed positioning in CSS.
relative positioning is relative to it's root where as absolute positioning is relative to it's parent.fixed position will be fixed at a particular place .In relative we can't give top,bottom,left.right value but incase of absolute and fixed we can define that.



# 13. What are the different data types in JavaScript?
  Data types in js are divided into 2 parts:primitive and non-primitive.Primitive data type are call by value that means if two variables refer to same value ,changing in 1 variable doesn't reflect changes in the other one ,as both of them refer to different memory location.Examples are string,char,number,BigInt,Boolean.On the other hand non-primitive data types are call by reference that means two variable with same value points to same memory location.Examples are array,object,method

# 14. Difference between null, undefined, and NaN.
Null means we are define a variable null value that can be consider as nothing .Undefined means we are creating a variable but not giving any value to it.Where as NaN is not a number .
Example:
let a =null
let a //undefined
let a =5/0 //NaN

# 15. Explain hoisting in JavaScript with an example.
To know about hoisting we need to know 2 things,
function declaration and function expression.
Both of them are used to declare function and perform task .The only difference it has is this hoisting property.
In case of function declaration we can call the function before it's actually declare and during run time js automatically moves function defination part to the top.
hello()
function hello(){
  //code
}
where as in case of function expression we store function inside an variable and we can't use that expression name before it's called
const hello = function(){
  //
}

# 16. What is the difference between map(), forEach(), and filter()?
All three of them are array methods.
forEach() will execute code for each array element and return undefined.it'll not change the orignal array.Map will also execute for each array element and return a new array of same length but doesn't change the orignal array.filter() will filterout the element based on condition.




Q3. Difference between let, const, and var?
let ,var,const three of them are used to define variables.var is the oldest one which has functinal scope issue.So currently we are using let and const.const is a fixed value and can't be reassign where as let can be reassign.
Q4. What is hoisting in JavaScript? Explain with an example.
Q5. Explain the concept of closures in JavaScript with a use case.

🔹 Coding Challenges

