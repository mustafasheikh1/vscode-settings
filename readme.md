# JS Coding Practices Phaedra Solution

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

### Variable Name
- A veriable name must be `camel casing` and self defining. example: `userId`, `fName`
- Use `let` and `const` instead of `var` in variable declaration
- Use `_` as a prefix for **private** variables, example: `_usr`.
- For perameters use `$` dollar prefix in the name. example
```js
    function addUser($user) {
        return $user;
    }
```

### Funtion
- A function name should be in `camal casing` just as a veriable.
- Use `_` as a prefix for **private** functions. example: `_getUser`
- Use `JsDoc` in functions like in the example below.
```js
    /**
    * @description For getting a user via its id
    * @param $id
    * @retruns User typeof Object
    */
    async function getUser($id) {
        return await User.get({ where: { _id: $id } });
    }
```
