Download Link: https://assignmentchef.com/product/solved-cse102-homework-1-function-to-read-three-integers-from-the-command-prompt
<br>
You will write a C file with the main function with three additional functions described below. Your Program will start calling part1, part 2 and part 3 functions in that order.  For each part, you will receive the inputs from the user and print the output to the console. Details of the parts are further discussed below.  Please pay attention to the output format. Any deviation from the shared format may be penalized regardless of the correct execution.

<strong>Part 1.</strong>  Your function will read three integers from the command prompt as coefficients of a quadratic equation and calculate the roots of the equation. If the roots are Real then Your program will print the equation and the roots to the console in descending order. If roots are complex numbers then the program will inform the user about the complex roots.

<strong>Example 1: </strong>

Please Enter the first coefficient:1

Please Enter the second coefficient:-3

Please Enter the third coefficient:-4

Output &gt;Your equation 1x^2 – 3x – 4 have real roots {4,-1}.

<strong>Example 2: </strong>

Please Enter the first coefficient:1

Please Enter the second coefficient:0

Please Enter the third coefficient:1

Output&gt; Your equation 1x^2 + 0x + 1  does not have any real roots. The function prototype is:

Function prototype is <strong>void</strong> <strong>find_root()</strong>

<strong>Part 2.</strong> Your second function will search for the roots by a numerical method called “Newton’s Algorithm”. This method is an iterative root-finding algorithm that produces better approximations to the roots of a real-valued function. You can find a very easy-to-understand introduction at <strong>Wikipedia</strong>. Furthermore,  web page at <strong>https://planetcalc.com/7748/</strong> can serve u as both a guideline and a validation resource.

In this function, you will again ask for three coefficients and an initial guess from the user and apply Newtons Method 5 times. In each step, you will compare the actual root and the estimated root (from the Newtons method) and print the difference. Unlike the first function, you don’t have to worry about complex roots. <strong>You can safely assume that users will not provide a function with complex roots</strong>.

<strong>Example</strong>:

Please Enter the first coefficient:1

Please Enter the second coefficient:-3

Please Enter the third coefficient:-4

Please Enter the initial: 10

Output &gt; Your equation is 1x^2 – 3x – 4 and iterations are

Step            x       f(x)                  Difference

<table width="291">

 <tbody>

  <tr>

   <td width="95">                x1</td>

   <td width="142">6.1176 15.0726</td>

   <td width="54">2.1176</td>

  </tr>

  <tr>

   <td width="95">                x2</td>

   <td width="142">4.4856 2.66366</td>

   <td width="54">0.4856</td>

  </tr>

  <tr>

   <td width="95">                x3</td>

   <td width="142">4.0395 0.19899</td>

   <td width="54">0.0395</td>

  </tr>

  <tr>

   <td width="95">                x4</td>

   <td width="142">4.0003 0.00154</td>

   <td width="54">0.0003</td>

  </tr>

  <tr>

   <td width="95">                x5</td>

   <td width="142">4.0000 0.00000</td>

   <td width="54">0.0000</td>

  </tr>

 </tbody>

</table>

Function prototype is <strong>void </strong><strong>find_newtonian_root()</strong>

<strong>Part 3.</strong> [30pts]  Given two integer you will calculate, divisibility of the first integer by the second one. If it is not, you will find the closest divisible integer. You will ask for the user input in the main function and pass the parameters to the find_multiple method. This function will return to the main function and it will be printed on the command prompt.




<strong>Example 1</strong>:

Enter the first integer: 76

Enter the second integer: 15

Output&gt; Closest number to 76 that is multiple of 15 is 75.




<strong>Example 2</strong>:

Enter the first integer: 76

Enter the second integer: 13

Output&gt; Closest number to 76 that is multiple of 15 is 78.




<strong>Example 3</strong>:

Enter the first integer: 76

Enter the second integer: 19

Output&gt; Closest number to 76 that is multiple of 15 is itself.

Function prototype is <strong>int </strong><strong>find_multiple_closest(</strong><strong>int </strong><strong>a, </strong><strong>int </strong><strong>b)</strong>