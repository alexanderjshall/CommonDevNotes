# Functions
## What Are They?
Functions are a type of data that modularises code, such that the same code can be executed any time where called. 
Functions are commonly referred to as opaque boxes, as they abstract away, or encapsulate, the internals of a task such that anything that uses the function can entrust

## Why are they important?
- Mathematical History: `f(x) = 2x + 3` is a (anonymous) function which takes `x` as a parameter and will evaluate the expression 2x + 3. This concept exists across mathematics (such as trigonometric functions).
- Re-usable Code: A function is responsible for a particular action, or group of actions. Where this task is to be done multiple times across a program, abstracting code in re-usable functions minimises the amount of code that needs to change.


## Common Terms
- `definition`: The code that the function will use when executed (i.e. what it does & how/where it is defined).
- `call` & `execute`: Running the code defined in the function definition.
- `return`: The output value of a function
- `scope`: The visibility of the function definition - variables in functions cannot be accessed from outside (and as such should be garbage collected after the function returns), but variables in the scope above the function can be accessed from inside.
- `parameters`: What values the function accepts from outside to use in the definition
- `arguments`: The actual values used for the parameters in any 
- `signature`: The combination of the paramater and return types (i.e. numbers) that define the function alongside the name.
- `overload`: The ability to have many functions of the same name with different signatures (language dependent)
- `higher-order` or `first-class`: Functions that either have functions as arguments, or return functions (where functions are just a type of data)
- `method`: a function that belongs to a class/object (and cannot be used outside of that context).

## Less Common Terms
- `side-effects`: When a function definition alters a variable outside of it's own scope thus altering a value that is not directly the value it returns.
- `pass-by-value`, `pass-by-address`, `pass-by-reference`: In most languages, function arguments are copied into the function scope, but not accessed directly, to prevent unintentional side effects, known as `pass-by-value`. Arguments can be passed by different types of variables in some languages that can refer to the same data, which can bypass this. `pass-by-reference` & `pass-by-address` means passing a reference to where the variable is stored in memory, which can then be dereferenced (in slightly different ways).



## Examples
(y will always be 13)
**Python**
Scope is defined by indentation.
```python
# define function <function_name> (<Parameters>):
def my_func(x):
  return 2 * x + 3 # return statement

y = my_func(5) #function call
```

**Typescript**
Scope defined by curly braces `{}`
```typescript
function myFunc(x: number) {
  return 2 * x + 3;
}

const y = myFunc(5);
```

**C#** (C languages are similar to this)
Scope defined by curly braces `{}`
```c#
public int MyFunc(int x) {
  return 2 * x + 3;
}
var y = MyFunc(5)
```

**F#**
This is a functional language. Notice that the arguments list is non distinctive, and the function auto-returns its last statement.
```f#
let myFunc x =
  2 * x + 3
```

**Ruby**
```ruby
def functionname(x)
   return 2 * x + 3
end
```
