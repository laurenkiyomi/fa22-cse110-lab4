<ol>
    <li>The following will be printed by line 12: 3. This is because 
    i is declared using the var keyword, so its scope is the whole function. </li>
    <li>Line 13 will print the following: 150. This is because discountedPrice is 
    declared using the var keyword, so its scope is the whole function. The last time 
    disountedPrice was declared and assigned was 300 * (1 - discount).</li>
    <li>Line 14 will print the following: 150. This is because finalPrice is 
    declared using the var keyword, so its scope is the whole function. The last time 
    finalPrice was reassigned a value was Math.round(150 * 100) / 100.</li>
    <li>[ 50, 100, 150 ]. The function will return this because all variables 
    are declared with the var keyword and thus have the function scope. For each 
    value in discounted, the finalPrice is recalculated and pushed into the discount 
    variable. Essentially half of each price in discounted is taken off and pushed 
    onto the discounted array in the same order as in the prices array.</li>
    <li>An error will occur because we are calling the i variable outside of its 
    scope. Because it is declared with the let keyword, its scope is only within the 
    for loop (block scope).</li>
    <li>An error will occur because we are calling the discountedPrice variable outside of its scope. Because it is declared with the let keyword, its scope is only within the for loop (block scope).</li>
    <li>150 will be printed to the console. This is because finalPrice is declared using the let keyword and has block scope, but since it is declared outside of the for loop, its scope is actually within the whole function. The last time finalPrice was reassigned a value was when calculating the final price of 300.</li>
    <li>[ 50, 100, 150 ]. The function will return this because none of the variables 
    declared are called outside of their scope. Similar to as described in question 7, 
    the discounted variable has block scope since it is declared with the let keyword, but its scope is the whole function since it is declared outside of the for loop.
    Thus this function has the same functionality as in question 4.</li>
    <li>An error will occur because we are calling the i variable outside of its 
    scope. Because it is declared with the let keyword, its scope is only within the 
    for loop (block scope).</li>
    <li>3 will be printed since it is the length of the prices array. No error will 
    occur because even though length is declared wth the const keyword, it is never 
    reassigned, and its scope is within the whole function because it is declared 
    outside of the for loop.</li>
    <li>[ 50, 100, 150 ]. The discounted and length variables do not cause errors 
    because they are never reassigned and their scope is the whole function since 
    they are declared outside of the for loop. The discounted array is added onto but the variable itself is never reassigned. i and discountedPrice are never called outside of its scope of the for loop. discountedPrice is never reassigned since 
    it is newly declared with each iteration of the for loop</li>
    <li>
        <ol>
            <li>student.name </li>
            <li>student["Grad Year"] </li>
            <li>student.greeting()</li>
            <li>student["Favorite Teacher"].name</li>
            <li>(student.courseLoad)[0]</li>
        </ol>
    </li>
    <li>
        <ol>
            <li>‘3’ + 2 = '32': integers map to their exact string representation</li>
            <li>‘3’ - 2 = 1: strings map to their integer representation</li>
            <li>3 + null = 3: null gets mapped to its integer representation (0)</li>
            <li>‘3’ + null = '3null': null gets mapped to its exact string representation</li>
            <li>true + 3 = 4: the boolean true gets mapped to its integer representation (1)</li>
            <li>false + null = 0: false and null get mapped to their integer representation (0)</li>
            <li>'3' + undefined = '3undefined': undefined maps to its exact string representation</li>
            <li>'3' - undefined = NaN: strings map to their integer representation, and 3 - undefined is undefined or NaN</li>
        </ol>
    </li>
    <li>
        <ol>
            <li>'2' > 1 is true: string '2' becomes a number 2</li>
            <li>'2' < '12' is false: '2' is greater than '1' in string comparison</li>
            <li>2 == '2' is true: '2' becomes a number 2</li>
            <li>2 === '2' is false: 2 and '2' are different types and no type conversion occurs with ===</li>
            <li>true == 2 is false: true becomes 1</li>
            <li>true === Boolean(2) is true: Boolean() converts 2 to the boolean true so true and true are of the same type and value</li>
        </ol>
    </li>
    <li>== compares variables after doing type conversion while === compares variables but doesn't do type conversion. So for === to return true, variables also have to be 
    the same type</li>
    <li>
        ```
            for (let property in statistics) {
                if (property.charAt(0) == 'r' || statistics[property] % 2 != 0) {
                    console.log(`${property}: ${statistics[property]}`);
                }
            }
        ```
    </li>
    <li>[2,4,6] will be returned. In modifyArray, for each value in [1,2,3], doSomething is called, which multipilies a given value by 2. Each value returned by doSomething is then pushed into newArr, which is returned by modifyArray.</li>
    <li>Refer to part2-question18.js</li>
    <li>1 4 3 2 is printed because 1 is printed, then 4, then 3 after a delay of 0 seconds, then 2 after a delay one second</li>
</ol>