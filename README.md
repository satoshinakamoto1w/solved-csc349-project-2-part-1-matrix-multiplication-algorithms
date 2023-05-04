Download Link: https://assignmentchef.com/product/solved-csc349-project-2-part-1-matrix-multiplication-algorithms
<br>
<strong><u>Requirement</u></strong>: to multiply A and B matrices, the <strong>number of columns in A must be equal to the number of rows in B</strong>. You must first do this validity check and throw an <strong><em>IllegalArgumentException</em></strong> type exception if the requirement is not met.

<u>Reminder</u>: the number of rows in a two-dimensional array <em>arr</em> is <em>arr.lenght</em> and the number of columns is <em>arr[0].length</em> (assuming all rows have the same number of elements, which is the case when representing a matrix).

<ul>

 <li><strong><em>main</em></strong>: In this method you will do the following (<em>no need to do any validity checks in main</em>):</li>

</ul>

<ol>

 <li>Prompt the user to enter the input-file’s name, then input the file-name and set up a scanner.</li>

</ol>




<ol start="2">

 <li>Create two 2-dimensional arrays for matrices A and B, and fill A and B with numbers, inputting values from the input-file as described below.</li>

</ol>




In the input-file you will have integer numbers only (there will not be any other symbols or signs). All numbers will be separated by whitespaces. The first two numbers will indicate the size of the A matrix (i.e. the number of rows and columns respectively), then values of the A matrix will follow (row after row, listing elements from left to right). After that, the next two numbers will indicate the size of the matrix B (i.e. the number of rows and columns respectively), then values of the B matrix will follow (row after row, listing elements from left to right). <em>You can assume that the 4 numbers representing A and B matrix-sizes will be positive numbers </em>(no need for validity check).




An example file-content is given below. Note that the data are shown in a clear and visually convenient look; however, there is <u>no formatting requirement</u> for the file, i.e. you should <strong><u>not</u></strong> assume/expect any mandatory line-breaks or empty lines.

<ul>

 <li><strong><em>3 </em></strong></li>

</ul>

<strong><em>    1 2 3 </em></strong>

<strong><em>    4 5 6 </em></strong>

<strong><em> </em></strong>

<ul>

 <li><strong><em>3 </em></strong></li>

</ul>

<strong><em>    1 2 3 </em></strong>

<ul>

 <li><strong><em>5 6 </em></strong></li>

</ul>

<strong><em>    7 8 9    </em></strong><strong><em>//No specific formatting: e.g. data may be saved all on one line: 2 3 1 2 3 4 5 6 3 3 1 2 3 4 5 6 7 8 9                        //                                              or they can be broken into lines in an arbitrary manner </em></strong>

Dr. Hasmik Gharibyan; CSC/CPE 349




<ol start="3">

 <li>Call <em>matrixProduct</em> method giving A and B matrices, and get the product-matrix (matrix C).</li>

</ol>




<u>Note</u>: be aware of a potential <em>IllegalArgumentException </em>from <em>matrixProduct</em>; if this happens, arrange to catch it and output an error message. <strong>You should not let the program crash. </strong>




<ol start="4">

 <li>Output the content of matrix C on the screen, in an appropriate “matrix”-format: <u>one line per</u> <u>matrix-row, separating values on the same row with space(s)</u>.</li>

</ol>

For the above example your output should look like this (<strong>only bold italic text is the output</strong>):




<strong><em>       Product matrix: </em></strong>

<strong><em>30  36  42</em></strong>                     //c<sub>1,1</sub>=1·1+2·4 + 3·7=30     c<sub>1,2</sub>=1·2+2·5 + 3·8=36     c<sub>1,3</sub>=1·3+2·6 + 3·9=42

<strong><em>66  81  96</em></strong>                     //c<sub>2,1</sub>=4·1+5·4 + 6·7=66     c<sub>2,2</sub>=4·2+5·5 + 6·8=81     c<sub>2,3</sub>=4·3+5·6 + 6·9=96

<strong> </strong>

<strong>Compile and run your program, test it thoroughly:  </strong>

Make sure the program works as expected and gives correct results (there are many online tools for matrix-multiplication so you can use one of them to check your data).

Try different size input matrices, including matrices that have only one row or only one column. Also make sure that your program works as expected when input matrices are not eligible/valid for matrix-multiplication (they do not meet the above mentioned size-requirement).


