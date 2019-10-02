# JavascriptTips

## Scope of variables
```javascript
function Test() {
    if(true){
      let hello = "Hello"; // Scope: block
      var world = "world"; // Scope: function
      something = "something"; // Scope: global
      console.log(hello); //Work
      console.log(world); //Work
      console.log(something); //Work
    }
    console.log(hello); //Not work
    console.log(world); //Work
    console.log(something); //Work
}

Test();

console.log(hello); //Not work
console.log(world); //Not work
console.log(something); //Work
```

## Create and launch function in one line
```javascript
(function test(){
    console.log("hello")
})();
```
