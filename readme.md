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

### Directories
- A folder must be in `kebab-case`. example: `common-components`.
- Use `@` prefix with the root level folders under src directory. example:
```
src/
 │－ @services
 │－ @components
 │－ @pages

```
### Filenames
- Just like a folder name a filename must also be in `kebab-case`. 
- Filename should be postfixed by the type of the file. example: `loading-spinner.component.js`, `utils.test.js`.

### Export Methods
- Always use centralized exports.