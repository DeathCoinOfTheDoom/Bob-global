
# Hyra global workflow
This is how we are working on our main and side project.
 - Produit 1
 - Produit 2

 ## Workflow git :
Naming branch : `<name>/<pr>` .
> Example :
```git commit -m "gl/CustomerAccountCreation```
>

How to commit ?
```git commit -m "<name>/explicit description of what you have made"```
>
Example :
> ```git commit -m "gl/delete card component"```


## Code :

ES6 syntax is everywhere if you are note familiar with it check : [here]( https://medium.freecodecamp.org/want-to-learn-es6-take-this-free-23-part-course-and-become-a-javascript-ninja-55002db1ff74)

**Variable naming :** 
Use `const` or `let` instead of `var`. Mainly `const` for 90% use cases.
We are using **camelCase** for our variable and **UPPERCASE** for global variable. 
Note that global variables need to be used in very special conditions do not abuse of this easy coding habit.
> Example : `const sagaMiddleware`

**Function**
We are using **PascalCase** for our class name and **camelCase** function name. Try to have only function with low logic inside in your code.
Immutable data structure.
> Immutable data cannot be changed once created, leading to much simpler application development, no defensive copying, and enabling advanced memoization and change detection techniques with simple logic.

-----------_Vue JS part

**Component**

Component must encapsulate a small part of logic. Just call it for its layout. 
It is recommended to initialize all the data properties that needs to be reactive upfront in the data option. For example, given the following template:

```html
 <div id="demo">
  <p v-class="green: validation.valid">{{message}}</p>
  <input v-model="message">
</div> 
```
```javascript
new Vue({
  el: '#demo',
  data: {
    message: '',
    validation: {
      valid: false
    }
  }
})
```

**Views**

About the `import` : please do not use absolute import there is an alias that refer to `src/`. You can call it as the following with the key `@`.
> Example : `@/components`

When you are using import syntax in es6 if you are specifying a file the will search the closest index.js file. 
> Example : `@/component` is equal to `@/component/index.js` 
