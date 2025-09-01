# Basics of JS
- Used for both client and server site.
- Node js =backend
- No need to define type (dynamically typed)

# ECMAScript
- Write standard for JS.
  
# var,let,const
- const is fixed , cann't reassign.
- var, let allow reassign.
- Use let over var due to scope issue in var.
- with out declaring var,let,const : we can declare variable.

# Datatypes
- Primitive (string,number,boolean,null,undefined,symbol,BigInt)
- Non-primitive (object,function,array)

# convert
- Number("33")=number
- Number("123abc") = NaN
- Number(null) = 0
- Number(undefined) = NaN
- Number(true)=1
- Number(false)=0
- Boolean(1) = true
- Boolean(0) = false
- Boolean('1') = false
- Boolean("Jina") = false

# operation
 - console.log("1" + 2) =12
 - console.log(1 + "2") =12
 - console.log("1" + 2 + 2) =122
 - console.log(2 + 2 + "1") =41
 - console.log(true) =true
 - console.log(+true) =1
 - console.log(true+ ) =error

# Stack,Heap
- Primitive uses Stack memory . (Copy) -> Changing value will not affect orignal value.
- Non-primitive uses Heap memory .(same reference) -> Changing value will affect orignal value as the reference is same.
  
# string
- use string interpolation : (`hello i am ${name} `);
- string methods : toUpperCase(),toLowerCase,CharAt(2),IndexOf('a"),substring(start-number,end-number),slice(2,4)

# Number 
- Define number by using object (new Number)
- Number methods : toFixed(),toPrecision(),toLocalString,

# Math
- methods : abs(),round(),ceil(),floor(),min(),max(),random()

# Date and Time
- create date by using (new Date())
- methods: toDateString(),toLocalString(),getMonth,getDay()
- create time (Date now())
- methods: getTime()

# Array
- resizable
- mix content
- methods: push(),pull(),pop(),unshift(),shift(),includes(),indexOf(),join(),slice(),splice()
  # few array concepts
  - Spread operator(...) will spread out array elements .
  - flat : will return all subarray into a single array.
  - shallow copy(share same reference)
  - Deep copy (new copy)

# Object 
- 
