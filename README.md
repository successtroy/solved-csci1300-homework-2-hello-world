Download Link: https://assignmentchef.com/product/solved-csci1300-homework-2-hello-world
<br>
<h1>Objectives</h1>

<ul>

 <li>Compile and run C++ code</li>

 <li>Take user inputs and produce outputs</li>

 <li>Understand C++ data types</li>

 <li>Perform arithmetic operations</li>

</ul>

<h1>Questions</h1>

<h2>Question 1: Hello World</h2>

The first program that we usually write in any language we’re learning is <em>Hello, World</em>​          ​. Create a program that prints “Hello, World!​ ” to the screen (the console window in Cloud9).​




Expected output

Hello, World!

The file should be named helloWorld.cpp​

Here are some suggested steps:

<h2>Step 1: Open an Empty File</h2>

In Cloud9, select File -&gt; New File​ . A new, blank file called Untitled1 will be opened.​

<h2>Step 2: Your First Code</h2>

Starting on line 1 in Untitled1, type the following code.

<h2>Step 3: Saving Your File</h2>

Save the file: go to ​File -&gt; Save As… ​A dialog box will open. Name it ​<strong>helloWorld.cpp</strong>​ and save it in the ​<strong>hmwk2</strong>​ folder.

Note: ​<em>make sure you save it with the .cpp extension or it will not compile correctly!</em>




The ​.cpp​ extension on the filename tells Cloud9 that the file should be read in the C++ programming language. Once you save it, the lines in the file should be color-coded to reflect what they do in the program. This is called syntax highlighting.




<strong>Important:</strong> You should save your work <u>frequently</u>​ in Cloud9 to avoid losing your work in the event of the program crashing. Also, you should take a backup of your Cloud 9 environment.

<h2>Step 4: Running Your Code</h2>

To run the program, click on the icon with the green arrow next to the word Run. If it works, you should see new terminal tab window open at the bottom. The title of the tab shows the file being run

(hmwk2/ helloWorld.cpp), and inside the window you should see “Running ….” (again the name and full path of the file), and underneath it, the output of our program: “Hello, World!​             ”​

<h2>Step 5: Running Your Code from Command Line</h2>

Move to the “bash” tab (the first tab in the bottom panel). Right-click again and Clear the Buffer.

Make sure you are inside the <strong>hmwk2</strong>​ directory. Type:​




<h3>$ g++ helloWorld.cpp -g -std=c++11</h3>




the -​ g option turns on debugging, which we will use later in the semester, so we should get used to it.

the -​ std=c++11 option makes sure that the c++ version used to run the program is c++ 11. If you don’t give this option then default version(which is usually C++98) is used.

This creates an executable called “a.out” (see figure below). You can run it by typing

<h3>$ ./a.out</h3>

Since no executable name was specified to g++, a.out is chosen by default. You can alternatively use the “-o” option to change the name :

$ g++ helloWorld.cpp -g -std=c++11 -o hello

creates an executable called “hello​ ” (see figure below). You can run it by typing​

<h3>$ ./hello</h3>

Notice the output in the same: Hello,​ world!,​ followed by the return of the prompt, for new commands.







<h2>Step 6: Submit to Moodle CodeRunner</h2>

Head over to Moodle to the link <a href="https://moodle.cs.colorado.edu/mod/quiz/view.php?id=45717"><strong>Homework 2 CodeRunne</strong></a>​ <a href="https://moodle.cs.colorado.edu/mod/quiz/view.php?id=45717"><strong>r</strong></a>. Submit your solution for the first​       problem and press the Check button. You will see a report on how your solution passed the tests, and the resulting score for the first problem. You can modify your code and re-submit (press “Check” again) as many times as you need to.

If the code runner says “incorrect”, click “show difference” button. It will highlight the differences between the expected output and the output your program produced. These outputs should be exactly the same, including upper/lower case, punctuation, and spaces. Otherwise, it’ll mark as incorrect. It’s a computer. It needs to be precise.




<strong>Question 2 : Hello You!  </strong>

If a program is more interactive, it’s fun! Create a program that takes a name and print prints “Hello, &lt;name&gt;!​           ”. Your output should be exactly the same as below, including the prompt​   for the user input.

Expected output (<strong>bold</strong>​ is user input)​

Enter your name:

<h2>Malvika</h2>

Hello, <strong>Malvika</strong>​ !​




The file should be named as helloYou.cpp​              . Don’t forget to head over to CodeRunner on​              Moodle and paste your solution in the answer box!




<h3>Question 3 Carnot efficiency</h3>

In thermodynamics, the Carnot efficiency is the maximum possible efficiency of a heat engine operating between two reservoirs at different temperatures. The Carnot efficiency is given as η = 1 − <em><sub>T</sub></em><em><sup>T</sup></em><em>H</em><em><u><sup>C</sup></u></em>

where  <em><sup>T</sup></em>​ ​<em>C</em> ​and <em><sup>T</sup></em>​ ​<em>H</em> ​are the absolute temperatures at the cold and hot reservoirs, respectively. Write a program that takes temperatures at the cold receiver(<em>T<sub>c </sub></em>) and hot receiver(<em>T<sub>h </sub></em>) as integer values, and computes ​ <sup>η</sup>​ the Carnot efficiency.​

Expected output (<strong>bold</strong>​ is user input)​

Enter cold reservoir temperature: <strong>10 </strong>

Enter hot reservoir temperature:

<h4>80</h4>

Carnot efficiency: 0.875




The file should be named as carnot.cpp​    . Don’t forget to head over to Code Runner on​             Moodle and paste your solution in the answer box!

<h3>Question 4 (10pt): Calculating sphere volume and area</h3>

Create a program that takes a radius as a floating-point value (as double​ )​ , and it prints both the volume and surface area of a sphere with the given radius. The formulas are: <em>volume</em> = π<em>r</em><sup>3 </sup> <sup> </sup> <em>surfaceArea</em> = 4π<em>r</em><sup>2 </sup> <sup> </sup>

For π , use M_PI​ from ​ #include &lt;cmath&gt;​




Expected output (<strong>bold</strong>​ is user input)​

<table width="624">

 <tbody>

  <tr>

   <td width="624">Enter a radius: <strong>3.3 </strong>Volume: 150.533Surface area: 136.848</td>

  </tr>

 </tbody>

</table>




The file should be named as sphereVolumeArea.cpp​      . Don’t forget to head over to Code​     Runner on Moodle and paste your solution in the answer box!




<h3>Question 5 (10pt): Temperature conversion</h3>

In science, the temperature is always described in Celsius, but in the U.S. we tend to use Fahrenheit. Create a program that takes user input for Fahrenheit (as double​ )​ and converts it into Celsius. The formula is:

<em>Celsius</em> = <u><sup>5</sup></u><sub>9</sub> (<em>Fahrenheit</em> − 32)

The calculated temperature Celsius values should be formatted with a two-digit precision as shown below. Fahrenheit value should be printed without any precision formatting applied.




Expected output (<strong>bold</strong>​ is user input)​

Enter a temperature in Fahrenheit:

<h4>76</h4>

The temperature 76 degrees Fahrenheit is <strong> </strong>​ 24.44​   degrees Celsius.




The file should be named as temperature.cpp​     . Don’t forget to head over to Code Runner on​             Moodle and paste your solution in the answer box!

<h3>Question 6 (10pt): Convert seconds</h3>

Write a program that takes a number of seconds as user input (as an integer​     )​ and converts it to hours, minutes, and seconds as shown below. You should convert the amount of time in such a way that maximizes the whole numbers of hours and minutes.




Expected output 1 (<strong>bold</strong>​ is user input)​

Enter a number of seconds:

<h4>60</h4>

0 hour(s) 1 minute(s) 0 second(s)




Expected output 2 (<strong>bold</strong>​ is user input)​

Enter a number of seconds:

<h4>3671</h4>

1 hour(s) 1 minute(s) 11 second(s)




The file should be named as convertSeconds.cpp​            . Don’t forget to head over to Code​     Runner on Moodle and paste your solution in the answer box!

<h3>Question 7 ): Population</h3>

The U.S. Census provides information about the current U.S. population as well as approximate rates of change. Using those rates and the current US population, write a program that takes a current population and computes the U.S. population in exactly one year (365 days). If you end up with a non-integer projected population, then round down to the nearest whole person.




Three rates of change are provided:

<ul>

 <li>There is a birth every 8 seconds</li>

 <li>There is a death every 12 seconds</li>

 <li>There is a new immigrant arriving in the US every 27 seconds</li>

</ul>







Expected output (<strong>bold</strong>​ is user input)​

Enter the current population:

<h4>1000000</h4>

The population in one year: 3482000




The file should be named as population.cpp​        . Don’t forget to head over to Code Runner on​             Moodle and paste your solution in the answer box!

<h1>Homework 2 checklist</h1>

Here is a checklist for submitting the assignment:

<ol>

 <li>Complete the <a href="https://moodle.cs.colorado.edu/mod/quiz/view.php?id=45722"><strong>conceptual reviews(mcq</strong></a><u>​ </u><a href="https://moodle.cs.colorado.edu/mod/quiz/view.php?id=45722"><strong>)</strong></a></li>

 <li>Complete the code <a href="https://moodle.cs.colorado.edu/mod/quiz/view.php?id=45717"><strong>Homework 2 CodeRunne</strong></a><u>​ </u><a href="https://moodle.cs.colorado.edu/mod/quiz/view.php?id=45717"><strong>r</strong></a></li>

 <li>Submit one zip file to <a href="https://moodle.cs.colorado.edu/mod/assign/view.php?id=45716"><strong>Homework </strong></a><u>​ </u><a href="https://moodle.cs.colorado.edu/mod/assign/view.php?id=45716"><strong>2</strong></a>. The zip file should be named, ​         <strong>zip</strong>​        . It​           should have the following 7 files:</li>

</ol>

○  <strong>helloWorld.cpp  ○     helloYou.cpp ○          carnot.cpp </strong>

<strong>○  sphereVolumeArea.cpp ○    temperature.cpp ○    convertSeconds.cpp ○         population.cpp</strong>