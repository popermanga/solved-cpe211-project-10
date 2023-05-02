Download Link: https://assignmentchef.com/product/solved-cpe211-project-10
<br>
<strong> </strong>

<h1>Project 10 Description</h1>




This project involves working with a one-dimensional array.  The maximum size for the one dimensional array is 50 elements.  The program will read floating point numbers from an input file and store them in a one dimensional array.  The following statistical values will be determined for the numbers read from the input file: The Mean (Average), The median (middle value), the standard deviation and the variance.  Formulas for these values are shown on page

<ol start="4">

 <li></li>

</ol>




<strong>The program is to use various functions to perform the necessary actions, and all functions are called from main.  No user defined function can call another user defined function.  Furthermore, all output (to the terminal) of the statistical values is to be performed in main – so functions must return the values they calculate. </strong>

<strong> </strong>

<strong>The <u>SIX</u> required functions that must be written are: 1) Sort numbers from low to high (first element of the array is the lowest value) 2) Find the average of the numbers 3) Find the median value 4) Find the variance  5) open an input file and 6) Read in the floating point numbers.  Other functions can be written if needed. </strong>




When opening the input file, all code is to be placed in the function that opens the input file.  The program is to continually prompt for an input file and attempt to open it until a file is successfully opened.  Look at the output of the sample solution for examples of invalid input files.




Information in the input file consists of 1 integer and several floating point numbers (1 per line).  The first number in the input file is an integer indicating the number of floating point values to read.  If the value is a number, it will be between 1 and 50 inclusive.




The program is to read (use extraction) the integer value representing the number of floating point values.  This read acts as a priming read on the file and is used to determine if a valid number was read, and this read can also be used to determine if the input file is empty as well.  The value read is used as the limit for the loop control variable when reading(use extraction) in the floating point values into the array.  Reading of the values is to be performed in a function. After a read of each number check the status of the input file stream to see if a number was correctly read or if the file stream is in the fail state.




After reading in the numbers, sort the numbers from low to high.  Use a function to perform this task.  This function is to have two parameters – the one dimensional array holding the numbers and an integer representing how many numbers are in the array.




After sorting the numbers, determine the average of the numbers.  Use a function to determine this value by passing in the array of floating point numbers and the integer representing how many numbers are in the array.  The average value is to be returned back to the caller of the function.




The median value is easy to determine once the numbers are sorted from highest to lowest. Use a function to calculate the median value.  The function returns the median value back to the caller of the function.

<strong>If the number of values in the array is odd</strong>, the median value is the middle value in the list of numbers.  To determine the index position of the middle value, divide the number of values in the array by 2 (use integer division).<strong>   </strong>

<strong>If the number of the values in the array is even, </strong>the median value is the average of the two middle values in the list of numbers.  The index values for these two middle values are the number of values in the array divided by 2 (use integer division) and (the number of values in the array divided by 2) – 1




Next calculate the variance of the numbers using the formula provided on page 4.  Remember, array indexing goes from 0 to dimension size -1.  The function is to return the variance calculated to the caller of the function (which is main).




In main, the standard deviation is calculated as the square root of the variance.




Once all values are calculated, output the results to the terminal as shown in the sample solution.




<h1>Project 10 Requirements</h1>

<strong> </strong>

<ul>

 <li>Program must contain at least the 6 functions mentioned in the description.</li>

</ul>




<ul>

 <li><strong>All statistical output statements are to be performed in main. </strong>ç ç</li>

</ul>

<strong> </strong>

<ul>

 <li><strong>User defined functions can be called from main only. </strong></li>

</ul>

<strong> </strong>

<ul>

 <li><strong>Identifying phrases for the statistical values are left justified in a field width of 25 </strong></li>

</ul>




<ul>

 <li>A function to open the input file is required. The function should <strong>continue to prompt the user for a valid input file</strong> name until a valid name has been entered or ctrl-c is typed to exit the program.</li>

</ul>




<ul>

 <li>To reset an input stream that failed to open use <strong>clear(); </strong><strong> </strong></li>

</ul>

<strong> </strong>

<strong><u>Project 10 Directions:</u></strong>




<ul>

 <li>Open a terminal window and move (cd) into the Project_10 directory created in the CPE211_FALL18 directory (This is the directory structure created in project 1.) The command for this is:  <strong>cd CPE211_FALL18/Project_10 (typing cd ~/CPE211/Project_10 </strong></li>

</ul>

<strong>works as well)</strong>.  You will need to modify the names as necessary to match your capitalization style for the two directories.




<ul>

 <li>Download all needed files from Canvas into this directory. Using a Text Editor (i.e. gedit), edit a file for project 10 (i.e. <strong>gedit Project_10.cpp</strong>).  Write your complete program so that it <strong><u>produces the desired output as shown by the provided solution executable.</u></strong></li>

</ul>




<ul>

 <li>Test the operation of your program using the sample data files provided and compare results from your program to those of the sample solution</li>

</ul>




<ul>

 <li>Several header files are required: <strong>string, iomanip, fstream and iostream</strong>.</li>

</ul>

<strong> </strong>

<strong><u>Project 10 Helpful Information</u></strong>

<strong> </strong>

<ul>

 <li>Statistical identifying phrases are output in a field width of 25 left justified</li>

 <li>Use setfill(‘.’) as an output manipulator to obtain the periods between the identifying phrases and the value output.</li>

 <li>Re-Use the function for opening the input file from previous projects.</li>

 <li>Most of the functions written will require at least a one-dimensional array parameter and an integer parameter representing how many numbers are in the array</li>

 <li>Use a defined constant for the maximum number of values possible for the array (50 for this program). Use this defined constant as necessary.</li>

 <li><strong>All message headings and bottom lines are 47 characters long. </strong></li>

 <li><strong>Use LOOPS for performing all of the necessary actions with the calculations. </strong></li>

 <li><strong>Input file can be empty. First value in the input file representing the number of floating point values to read may be a number or some other character. </strong></li>

 <li><strong>Program should test for invalid data possibilities when reading the floating point values </strong> <strong>Program needs to be able to handle invalid file names </strong></li>

</ul>

<strong> </strong>

<h1>Project 10 Assumptions</h1>

<strong> </strong>

<ul>

 <li>Each number is on a separate line and all values are read using extraction.</li>

 <li>Look at input files. Blank lines may exist in the input files</li>

</ul>

<strong> </strong>

<strong> </strong>

<strong><u>Project 10 Formulas</u> </strong>

<strong>The cmath header file:</strong>  This header file contains definitions for various math functions including the pow(x,y) function.  The pow(x,y) function calculates the value of x<sup>y</sup>.  If pow(x,y) is used when calculating the variance, y must be the integer value of 2.




<h1>Formulas Required</h1>

<em>n</em>1

<em>Sum</em>: <em>X</em><em>sum</em><em>X</em><em>i</em>

<em>i</em>0

<em>X</em><em>sum</em>

<em>Average</em>: <em>X</em><em>avg </em> <em>n</em>

var<em>iance</em>: var1<em>n</em><em>ni</em><sub></sub>01(<em>X</em><em>i </em><em>X</em><em>avg</em>)2



<em>S</em>tan<em>dardDeviation</em>:  var

<strong><u>Note: the summations go from 0 to n-1 where n is the number of floating</u></strong><strong> <u>point values.  This terminology is used because the numbers are stored in</u> <u>the array starting with index value 0 to index value n-1.</u></strong>