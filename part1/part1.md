1. The final value of `i` which equals `(prices.length - 1)` will be printed at line 11, since the declaration of `var` does not have block scope and `i` is function-scoped in this case.
2. The final value of `discountedPrice` will be printed at line 12, since the declaration of `var` does not have block scope and `discountedPrice` is function-scoped in this case.
3. The final value of `finalPrice` calculated from the loop will be printed at line 13, since the declaration of `var` does not have block scope and `finalPrice` is function-scoped in this case.
4. The function will return `[50, 100, 150]`. Since the discount is `0.5`, the loop goes through each price and calculates a new `discountedPrice` by multiplying each value in the price array by `0.5`.
Then the `finalPrice` of each `discountedPrice` is the same as before because the rounding process has no effect since the varaibles are already rounded. Therefore, each `finalPrice` calculated
from the loop will be pushed to the `discounted` array, being `[50, 100, 150]`.
5. There would be an error at line 11. Although `let i` is visually outside of the `{...}`, the variable is still considered a part of the block due to the specialness of `for` construction. 
Therefore, the variable `i` is only visible inside the scope of the loop.
6. There would be an error at line 12, since `let discountedPrice` is declared inside the for loop and thus the variable is only visible inside the scope of the loop.
7. The final value of `finalPrice` calculated from the loop will be printed at line 13, since `let finalPrice` is declared outside the for loop, and therefore the variable is function-scoped.
8. The function would return nothing and will print error messages. Since there are multiple variables that we could not access because they are out of scope, there would be no return value
and error messages like "i is not defined" will be printed.
9. There would be an error at line 11. Although `let i` is visually outside of the `{...}`, the variable is still considered a part of the block due to the specialness of `for` construction. 
Therefore, the variable `i` is only visible inside the scope of the loop.
10. There would be an error at line 12, since we are trying to modify the value for `finalPrice` at line 7, which is declared as a `const` and this means we cannot change its value.
So we will never be able to reach line 12 and nothing will be printed out besides the error messages.
11. There would be an error at line 13, since we are trying to modify the value for `finalPrice` at line 7, which is declared as a `const` and this means we cannot change its value.
So we will never be able to reach line 13 and nothing will be printed out besides the error messages.
12. The function would return nothing and will print error messages. The script stops at line 7 because we are trying to modify a `const` variable, so nothing will be returned except for printing error messages.<br/>

13. Given the above Object, write the notation for:<br/>
A. `student.name`  
B. `student['Grad Year']`  
C. `student.greeting()`  
D. `student['Favorite Teacher'].name`  
E. `student.courseLoad[0]`

14. Arithmetic <br/>
A. `32`: `2` gets type converted to string `'2'`, and appending it to string `'3'` we get `32`. <br/>
B. `1`: Since `-` is not a string operator, `3` gets type converted to a number, and numerical operation `3 - 2 = 1` got performed.  <br/>
C. `3`: Since `3` is a number, `null` gets type converted to number `0`, and numerical operation `3 + 0 = 3` got performed.  <br/>
D. `3null`: `null` gets converted to a string and is appended to string `'3'` <br/>
E. `4`: `true` gets numerically converted to `1` and adding it to number `3`.<br/>
F. `0`: `false` gets numerically converted to `0` and `null` also gets converted to number `0`, adding these two up gives `0`.<br/>
G. `3undefined`: `undefined` gets type converted to string `'undefined'` and is appended to stirng `'3'`.<br/>
H. `NaN`:  Since `-` is not a string operator, `undefined` gets numerically converted to `NaN` and `"3"` gets converted to number '3', then `3 - NaN = NaN` got performed.<br/>

15. Comparison <br/>
A. `true`: String `'2'` gets converted to number `2`, and `2` is greater than `1`.<br/>
B. `false`: JavaScript uses “lexicographical” order to compare strings, so `'2'` with a higher ACII value than `'1'` will result in `'12' < '2'`.<br/>
C. `true`: `==` checks the equality with type conversion, so `'2'` is converted to number `2` and `2 == 2` is `true`. <br/>
D. `false`: `===` checks the equality without type conversion, so `2 === '2'` immediately returns false because their types are different<br/>
E. `false`: `true` gets converted to number `1` and therefore `1 == 2` is `false`.<br/>
F. `true`: `Boolean(2)` evaluates to `true`, and we checks equality without type conversion. Since both sides are of boolean values, `true === true` returns `true`.<br/>

16. Explain the difference between the == and === operators.<br/>
A regular equality check `==` checks the equality with type conversion, meaning we can compare any two values no matter of their data types. As long as `a` and `b` are equal in value after type conversion, `a == b` will return `true`.
A strict equality operator `===` checks the equality without type conversion, meaning we are comparing `a` and `b` of two different data types, then `a === b` immediately returns false without attempting to convert them.

17. `How are you?` will be printed. For the first if statement, `2 == true` evaluates to `false` because `true` is numerically equivalent to `1` and `2 != 1`. So `Hello!` will not be
printed. Then we look at the second if statement, and `2` gets converted to a boolean value `true`, so we go into this if statement and `How are you?` gets printed out as a result.

18. see .js file uploaded

19. The result will be `[6,8,10]`. First the function `modifyArray` creates an empty array `newArr`. Then we go into the for loop to iterates through `[1,2,3]`. For each value in the array, `doSomething` gets
called such that the number adds `2` in its value, and then the whole thing gets multiplied by `2`. So the overall operation for each number `num` in the array is `(nunm + 2) * 2`. Working through each number in the array in this way, we get `[6,8,10]` as 
the final value of `newArr` being returned.

20. see .js file uploaded

21. The output is:  
`1`  
`4`  
`3`  
`2`  
First, `1` and `4` are printed out as`printNums` executes. After that, the second `setTimeout` executes because there is no delays, and `3` is printed. 
Lastly, the code in the first `setTimeout` executes after delays in time, and `2` is printed. 


