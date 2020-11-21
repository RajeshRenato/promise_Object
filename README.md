# promiseObject
wrapper class for promises in object form


```javascript
Promise.object = require('@Renato/promiseObject')
//dependency
    // "@Renato/promiseObject": "git+https://github.com/RajeshRenato/promise_object.git"
let s = Promise.resolve(1);

let p = {
    k: Promise.resolve(2),
    j: Promise.resolve(3)
};

let r = {
    p,
    k: Promise.resolve(2),
    j: Promise.resolve(3)
};

let q = [Promise.resolve(4), Promise.resolve(5)]


let a = {s,r,q}

Promise.object(a).then(res=>{
    console.log(res)
})

})
```
