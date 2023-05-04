Download Link: https://assignmentchef.com/product/solved-csc110-fundamentals-of-programming-i-assignment-7-objects-searching-sorting
<br>
<h1>Learning outcomes</h1>

When you have completed this assignment, you will understand:

<ul>

 <li>How to create an <em>instance</em> of a <em>class</em> (object instantiation).</li>

 <li>How to invoke an <em>object’s instance methods</em>.</li>

 <li>How to create and use an <em>array</em> of <em>objects</em>.</li>

 <li>How to <em>search</em> and <em>sort</em> through data in an array.</li>

</ul>




In this assignment you will be writing methods in a Java program UvicOrganizer.java. Your program will use UvicCourse objects. Download the <strong>UvicCourse.java</strong> file and save it in the same directory as the UvicOrganizer.java file.

UvicCourse objects have three instance variables, String dept, int num, and String title, as shown below. Suppose our course, CSC 110, was represented as an instance of a UvicCourse called c1, it would look like the following:




In this assignment, you will use a Scanner to read through a text file containing course data, and fill an array of UvicCourses with this data. You will then create methods to print, search and sort through the array.

<strong><em>             </em></strong>

<strong><em>Your program must: </em></strong>

<ol>

 <li>Follow the <a href="https://connex.csc.uvic.ca/access/content/group/c695ec2f-7536-40a4-8ddc-eec4c5c20d41/Assignment%20Resources/Assignment7/UvicOrganizer.html">specification document</a><a href="https://connex.csc.uvic.ca/access/content/group/c695ec2f-7536-40a4-8ddc-eec4c5c20d41/Assignment%20Resources/Assignment7/UvicOrganizer.html">.</a></li>

 <li>Ask the user to enter the name of the input file. Note that the marker can use a different data file than the examples provided in the Appendex. The data file will have exactly the same format (i.e., same columns, with each row having the same number of items) but it may contain more or fewer rows. <strong><em>Continue to ask for another input filename if the one entered is not valid.</em></strong></li>

</ol>

<h2><strong>Input file format </strong>(example:  smallList.txt)</h2>

<ul>

 <li>The first line contains the number of UvicCourse data elements are contained in the file (the total number of courses to put into the array)</li>

 <li>Each remaining line contains the department name, followed by the course number. The remaining words on each line make up the course’s title.</li>

</ul>




<ol start="3">

 <li>After linking a Scanner to an input file, write the method <strong>makeArray</strong>, that accepts the Scanner as a parameter, and then creates and fills a UvicCourse array with all of the UvicCourse data contained in the file the Scanner is linked to. The method then returns the array.</li>

</ol>




<ol start="4">

 <li>Using the array returned from the <strong>makeArray</strong> method, create and test all of the other methods according to the specification document. Examples of how to test these methods are shown in the Appendix.</li>

</ol>

<strong> </strong>

<strong> </strong>

<h1>Marking</h1>

Your mark will be based on the following criteria:

<ul>

 <li>Your code <em>must compile and run</em>. Some examples of how to test your methods, along with expected output, are outlined in <strong>Appendix A.</strong></li>

 <li>Your code must conform to all the requirements mentioned in the <a href="https://connex.csc.uvic.ca/access/content/group/c695ec2f-7536-40a4-8ddc-eec4c5c20d41/Assignment%20Resources/Assignment7/UvicOrganizer.html">specification document</a><a href="https://connex.csc.uvic.ca/access/content/group/c695ec2f-7536-40a4-8ddc-eec4c5c20d41/Assignment%20Resources/Assignment7/UvicOrganizer.html">.</a></li>

 <li>Test each of the required methods to ensure each one functions correctly.</li>

 <li>Your code must follow the guidelines outlined in Style_Guidelines.pdf, found through the Lectures &amp; Stuff link in the Lab Resources folder on connex. You may notice that the specification document provides some very nice comments you are welcome to borrow.</li>

</ul>

<strong><u>Appendix A – Testing your code</u></strong>

<strong>Getting started setting up the </strong><em>main</em><strong> method: </strong>

Your main method will have two Scanners. The first Scanner is used to read in user input from the console (user entries underlined in red):




The second Scanner scans the contents of a file. If the file cannot be found, the program prompts the user to enter another file name, until the second Scanner is successfully linked to a file (as shown above).










<em>makeArray</em> <strong>method:</strong>

Now that you have a Scanner linked to a text file, the next step is to copy all of the contents of the file into an array of UvicCourses.

Input files will all have the following format:

<ul>

 <li>The first line contains the number of UvicCourse data elements that are contained in the file (the total number of courses to put into the array)</li>

 <li>Each remaining line contains the department name, followed by the course number. The remaining words on each line make up the course’s title.</li>

</ul>

Assuming we have linked a Scanner to the file <strong>smallList.txt</strong>:




Each line of data can be used to create a single instance of a UvicCourse. For example, the first line would create the following (in this case named c1):




Then each UvicCourse is inserted into an array, creating the following array of UvicCourse objects:




<em>printArray</em> <strong>method: </strong>

Given an array of UvicCourse objects, the method prints out information about each element in the array.

Given the following array (read in from <strong>smallList.txt</strong>):







Calling this method and passing in the array above produces the following output:




<em>listCoursesInDept</em> <strong>method: </strong>

Given an array of UvicCourses and a department name, this method prints out all UvicCourses in the array that match the department.

Example:

<strong>courseArray (read in from </strong>firstYearList.txt<strong>): </strong>

Given the above courseArray, and 3 lines of code, the following output is produced (input entered by the user into the console is underlined in red):

<strong>             </strong>

<em>listCoursesByDeptAndYear</em> <strong>method: </strong>

Given an array of UvicCourses and a department name, this method prints out all UvicCourses in the array that match the department.

Example:

<strong>courseArray (read in from file medList.txt): </strong>

Given the above courseArray, and 5 lines of code, the following output is produced (input entered by the user into the console is underlined in red):

<strong>             </strong>

<em>sortByNumber</em> <strong>method: </strong>

Given an array of UvicCourses, this method sorts the array by the <strong>num</strong> instance variable. Example:

<strong>courseArray (read in from file medList.txt): </strong>




Call your completed <strong>printArray</strong> method before and after sorting to ensure the array has been properly sorted.

<strong> </strong>