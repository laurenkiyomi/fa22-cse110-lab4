<ol>
    <li>The bug was that num1 and num2 were of type string, so result was 
    basically the two strings concatenated together</li>
    <li>I'd fix it by converting num1 and num2 to integers before adding them 
    together. I changed line 10 to `let result = Number(num1) + Number(num2)`.</li>
</ol>