
# h2w
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
> ```git commit -m "gl/Delete Card component"```


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
