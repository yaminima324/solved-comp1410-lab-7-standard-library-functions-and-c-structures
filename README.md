Download Link: https://assignmentchef.com/product/solved-comp1410-lab-7-standard-library-functions-and-c-structures
<br>
<strong>Objective: (a) </strong>Learn more about the functions from the standard libraries.  There are a great many standard functions that are included with C compilers. These functions are designed to carry out various common and repeatedly performed tasks by the C programmers. Having a good understanding about these functions and properly utilizing them can greatly reduce the coding time for large and complex programs. <strong>(b)</strong> In C, a structure (<strong>struct</strong>) is an <em>aggregate data type</em> that allows us to group one or more variables of different data type together to form a new, more complex data type. In this lab we will practice some simple usage of structure along with some more practice using strings.

<strong>Work to do: </strong>

<ol>

 <li>Go to the web page: http://www.cplusplus.com/reference/clibrary/. Click on various C libraries and study the functions, including what are their purposes, type of their return values, the parameter lists, examples of uses, etc. In particular, review the functions in the following headers: &lt;ctype.h&gt;, &lt;math.h&gt;, stdio.h&gt;, &lt;stdlib.h&gt;, &lt;string.h&gt; and &lt;time.h&gt;.</li>

 <li>In a simple way, define your own versions of the flowing functions. Test your functions by writing a main(). (Call the program Lab7a.c) Do not forget to document assumptions for each function that you program.</li>

</ol>

int AtoI ( const char * str ); int StrCmp ( const char * str1, const char * str2 ); char * StrCpy ( char * destination, const char * source ); char * StrCat ( char * destination, const char * source ); char * StrChr ( char * str, int character );

<ol start="3">

 <li>Write a C program called “Lab7b.c” to accomplish the following:</li>

</ol>

<h1>Outside of main()</h1>

1) Define a C structure named myWord with the following members:

<ol>

 <li>char Word[21] ; b. int Length ;</li>

</ol>

<h1>Inside of main()</h1>

<ul>

 <li>Declare an array named WordList of type myWord with size 20.</li>

</ul>




<ul>

 <li>Declare a string as follows:</li>

</ul>

char myString[] = “the cat in the hat jumped over the lazy

<h2>fox”;</h2>

<ul>

 <li>Use library function strtok() to extract each word from myString and store it in the WordList. (Assume space is the only delimiter separating the words).</li>

</ul>




<ul>

 <li>Use the library function strlen() to find the length of each word and store the value in the member Length.</li>

</ul>




Note: To access the Word array inside WordList use the “dot” operator.  e.g. strcpy(WordList[n].Word, “hello”);

[If you prefer, you could maintain an integer variable to keep a record of the number of words extracted].

<ul>

 <li>Print the contents of the WordList.</li>

 <li>Sort the WordList in alphabetical order. (Hint: use a simple <em>bubble sort</em> algorithm and use the library function strcmp() to compare two words.)</li>

 <li>Print the contents of the now sorted WordList.</li>

</ul>

<strong>Note: you should test your program with different </strong><strong>myString</strong><strong> values, including an empty string. </strong>

<strong>Summary of the lab requirements:  </strong>You must write two programs for this lab, namely Lab7a.c (for step 2) and Lab7b.c (for step 3).  Be prepared to demonstrate both programs with appropriate test input examples.