1. `i` is declared as a `var` variable, which means it is visible through code blocks within the same function. In this case `i` is increased in the for loop until it is greater than or equal to the length of `prices`. At line 12, `i` is still visible and is equal to 3. </br>**The output at line 12 is: 3**
2. `discountedPrice` is declared as a `var` variable, which means it is visible through code blocks within the same function. In this case `discountedPrice` is calculated by multiplying the price at index `i` by the discount passed in as the third argument to the `discountPrices` function. In the last iteration of the for loop, `discountedPrice` is set equal to `prices[2] * (1 - discount)`. This is equal to 150. At line 13, `discountedPrice` is still visible and is equal to 150. </br>**The output at line 13 is: 150**
3. `finalPrice` is declared as a `var` variable, which means it is visible through code blocks within the same function. In this case `discountedPrice` is calculated by rounding the `discountedPrice` to the nearest integer. In the last iteration of the for loop, `discountedPrice` is set equal to `prices[2] * (1 - discount)`. This is equal to 150. `finalPrice` is set equal to `Math.round(discountedPrice * 100) / 100`, which also equals 150. At line 14, `finalPrice` is still visible and is equal to 150. </br>**The output at line 14 is: 150** 
4. `discounted` is declared as a `var` variable, which means it is visible through code blocks within the same function. In each iteration of the for loop, `finalPrice` is pushed to `discounted`. At line 16, `discountedPrice` is still visible and contains three prices. </br>**The output is: [ 50, 100, 150 ]**
5. `i` is declared as a `let` variable within the for loop, which means it is only visible inside the for loop. This code causes an error because there is no such variable `i` at line 12.
6. `discountedPrice` is also declared as a `let` variable within the for loop, which means it is only visible inside the for loop. This code causes an error because there is no such variable `discountedPrice` at line 13.
7. Even though `finalPrice` is defined as a let variable, you can reassigned it's value within the if statement because it have a function-scope. Therefore, `finalPrice` is equal to 150 when the for loop is finished and **the output at line 14 is 150.**
8. **The output is: [50, 100, 150]** Even though the `discount` array is defined as let, you can still push to the array. Therefore, `finalPrice` is pushed to `discounted` in each iteration of the for loop.
9. `i` is declared as a `let` variable within the for loop, which means it is only visible inside the for loop. This code causes an error because there is no such variable `i` at line 11.
10. **This code will output 3 at line 12**. This is because `length` is defined as a constant value outside of the if statement and is set to equal the length of the `prices` array, which is 3.
11. **The output is: [50, 100, 150]** Even though the `discount` array is defined as a const, you can still push to the array. Therefore, `finalPrice` is pushed to `discounted` in each iteration of the for loop.
12. 
- A. We can access the value of the name property in the student object using `alert( student.name );` or `console.log( student.name );`, ( `student.name` ).
- B. We can access the value of the Grad Year property in the student object using `alert( student['Grad Year'] );` or `console.log( student['Grad Year'] );`, ( `student['Grad Year']` ).
- C. We can call the function for the greeting property in the student object using `console.log( student.greeting() );`, ( `student.greeting` ).
- D. We can access the name property of the object in the Favorite Teacher property in student using `console.log( student['Favorite Teacher'].name );`, ( `student['Favorite Teacher'].name` ).
- E. We can access index zero in the array of the courseLoad property of the student object using `console.log( student.courseLoad[0] );`, ( `student.courseLoad[0]` ).
13. 
- A. The output is **`'32'`**. This is because integers map to their exact string representation.
- B. The output is **`1`**. This is because the string was converted to int to complete the expression.
- C. The output is **`3`**. This is because null is treated as zero since the ASCII null is represented as 0x00.
- D. The output is **`'3null'`**. This is because null is treated as a string since the first argument is a string.
- E. The output is **`4`**. This is because true maps to 1 to complete the expression.
- F. The output is **`0`**. This is because false maps to 0 and null maps to 0 and are added together to complete the expression.
- G. The output is **`'3undefined'`**. This is because undefined is treated as a string since the first argument is a string, just like null was treated in part D.
- H. The output is **`NaN`**. This is because NaN is a numeric data type that means an undefined value, and this is returned because '3' is convert to a numerical value and the answer to this expression cannot be represented.
14. 
- A. The output is **`true`**. This is because '2' is mapped to its exact integer representation to complete the logical expression, and 2 is greater than 1.
- B. The output is **`false`**. This is because the the first character of both strings is compared and '1' is less than '2', so the expression is false.
- C. The output is **`true`**. This is because '2' is mapped to its exact integer representation to complete the logical expression, and 2 is equal to 2.
- D. The output is **`false`**. This is because `===` checks the equality between the values without type conversion, so false is returned because the types of 2 and '2' are different.
- E. The output is **`false`**. This is because true maps to 1 to complete the expression and 1 is not equal to 2.
- F. The output is **`true`**. This is because Boolean(2) evaluated to true and is equal to true. The Boolean() conversion returns true when converting a number.
15. The difference between the `==` and `===` operators is that `==` converts different types of operands to numbers, and `===` checks the equality without type conversion. For example, `0 == false` evaluates to true because false is mapped to 0, but `0 === false` because the operands are different types.
