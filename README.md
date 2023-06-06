<p align="center">
  <img src="https://pixabay.com/get/g20467c66325722c38733e743c7488ba03621312329bada765ceacd9cd1ef0a6264d389d314e174dae86f84aee1990d04_640.png" alt="예시 이미지" width="300" height="300">
</p>

# Let's go My PromisetileLibrarys 🚀

## Technology 🔧
![mocha](https://img.shields.io/badge/mocha-8D6748?&logo=mocha&logoColor=white)
![webpack](https://img.shields.io/badge/webpack-8DD6F9?&logo=webpack&logoColor=white&textColor=white)
![rollup](https://img.shields.io/badge/rollup-EC4A3F?&logo=rollup.js&logoColor=white)

### Function Introduction

_If you go to the link, you can see the base for each promise method I made! 🙏_

[Promise All](https://github.com/WooHyucks/Let-s-go-my-PromisetileLibrarys/blob/PromisetileLibrarys/PromiseOption/src/Promise.All.js) 
---
> The Promise.all() method returns a promise that will be restored after all promises given to the iterable object have fulfilled, or when the promise is delayed in voltage. If one of the given promises is waived, it uses the reason of the first rejected promise to consume itself as well.

```
const promise1 = Promise.resolve(3);
const promise2 = 42;
const promise3 = new Promise((resolve, reject) => {
  setTimeout(resolve, 100, 'foo');
});

Promise.all([promise1, promise2, promise3]).then((values) => {
  console.log(values);
});
// Expected output: Array [3, 42, "foo"]
``` 


[Promise Any](https://github.com/WooHyucks/Let-s-go-my-PromisetileLibrarys/blob/PromisetileLibrarys/PromiseOption/src/Promise.Any.js)
---
> The Promise.any() static method takes an iterable of promises as input and returns a single Promise. This returned promise fulfills when any of the input's promises fulfills, with this first fulfillment value. It rejects when all of the input's promises reject (including when an empty iterable is passed), with an AggregateError containing an array of rejection reasons.

```
const promise1 = Promise.reject(0);
const promise2 = new Promise((resolve) => setTimeout(resolve, 100, 'quick'));
const promise3 = new Promise((resolve) => setTimeout(resolve, 500, 'slow'));

const promises = [promise1, promise2, promise3];

Promise.any(promises).then((value) => console.log(value));

// Expected output: "quick"
``` 

[Promise Sequential](https://github.com/WooHyucks/Let-s-go-my-PromisetileLibrarys/blob/PromisetileLibrarys/PromiseOption/src/Promise.sequential.js)
---
> There is only one difference between Promise.all usage and promise-sequential usage:promise-sequential receive an Array of functions that each returns a promise.

>usage
```
const sequential = require('promise-sequential');
 
const items = [
  () => new Promise( ... )
  () => new Promise( ... )
  () => new Promise( ... )
];
 
sequential(items)
.then(res => {
  // ...
})
.catch(err => {
  // ...
})
``` 



[Sleep](https://github.com/WooHyucks/Let-s-go-my-PromisetileLibrarys/blob/PromisetileLibrarys/PromiseOption/src/Sleep.js)
---



      
