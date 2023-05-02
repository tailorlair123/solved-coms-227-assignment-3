Download Link: https://assignmentchef.com/product/solved-coms-227-assignment-3
<br>
<span style="font-size: 2.61792em; letter-spacing: -1px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">Overview</span>

<span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">In this homework, you need to write two classes (namely Maze, MazeCell), whose skeleton codes are given under package </span><em style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">hw3</em><span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;"> in the zip file. The classes under packages </span><em style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">maze</em><span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;"> and </span><em style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">strategy</em><span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;"> you must NOT modify. You may modify RunSearcher under the </span><em style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">ui</em><span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;"> package to run the search for different mazes or to test your code. This is the class that you use to run the whole program. You don’t submit RunSearcher. The </span><em style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">forwardSearch</em><span style="font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;"> method in the RunSearcher class should be quite interesting. If you are curious, you may want to read it at your leisure to figure out how the search actually works.</span>




The classes under <em>strategy </em>are different comparators that allow a cell’s neighbors to be searched in different orders, and are used by the <em>forwardSearch</em> method. They are included here for completeness and for fun, but you don’t have to read them.  <strong><em>The main purpose of this assignment is to help you practice arrays (especially 2-D arrays), loops, and ArrayLists</em></strong>. So you should focus only on package <em>hw3</em>.




The <em>maze</em> package contains classes mostly for graphical user interface. Check them out only if you are curious. Status in package <em>maze</em> represents an enum type, which is fairly easy to use.

Here are some examples:  private Status status; // use Status as type  or,

status = Status.WALL; // set status to be a WALL or,

if(status==Status.Wall) // check if status is WALL




There are two classes in hw3 that you need to complete. Descriptions about these classes are given in the java doc. <em><u>Make sure to read the javadoc carefully so as to follow exactly the</u> <u>specifications</u></em><u>.</u>







<h1>Sample usage</h1>




A good way to think about the specification is to try to write some simple test cases and think about what behavior you expect to see. Some basic tests on MazeCell and the Maze class are given in a class called <strong>MazeAndMazeCellTest.java</strong> in package <em>ui</em>.  You should expand the test cases to thoroughly test your classes.







<h1>Suggestions for getting started</h1>

<strong> </strong>

<em>Smart developers don’t try to write all the code and then try to find dozens of errors all at once; they work <strong>incrementally</strong> and test every new feature as it’s written.   Here is a rough guide for how an experienced coder might go about creating a class such as this one: </em>







<ol>

 <li>Import the given zip file to Eclipse. See section <strong>Importing the sample code</strong> below for instructions.</li>

</ol>




<ol start="2">

 <li>Start on the MazeCell class first. Look at each method.  Mentally classify it as either an <em>accessor</em> (returns some information without modifying the object) or a <em>mutator</em> (modifies the object, usually returning <strong><sub>void</sub></strong>).  The accessors will give you a lot of hints about what instance variables you need. Write your own test codes, or use and expand <strong>java</strong>, to make sure your methods are implemented correctly.</li>

</ol>




<ol start="3">

 <li>Similarly, work on the Maze class.</li>

</ol>







<h1>Testing and the SpecChecker</h1>




As always, you should try to work incrementally and write tests for your code as you develop it. <strong><sub> </sub></strong>




We will provide a basic SpecChecker, but<strong> it will not perform any functional tests of your code</strong>.  At this point in the course, you are expected to be able to read the specfications, ask questions when things require clarification, and write your own unit tests.  Since the test code is not a required part of this assignment and does not need to be turned in, <strong>you are welcome to post your test code on Piazza for others to check, use and discuss.  </strong>




The SpecChecker will verify the class names and packages, the public method names and return types, and the types of the parameters. If your class structure conforms to the spec, you should see a message similar to this in the console output:




x out of x tests pass.




This SpecChecker will also offer to create a zip file for you that will package up the two required classes.  Remember that your instance variables should always be declared <strong><sub>private</sub></strong>, and if you want to add any additional “helper” methods that are not specified, they must be declared <strong><sub>private</sub></strong> as well.




See the document “SpecChecker HOWTO”, which can be found in the Piazza pinned messages under “Syllabus, office hours, useful links” if don’t remember how to import and run a SpecChecker.




<h1>Importing the sample code</h1>

<ol>

 <li>Download the zip file. You don’t need to unzip it.</li>

 <li>In Eclipse, go to File -&gt; Import -&gt; General -&gt; Existing Projects into Workspace, click Next.</li>

 <li>Click the radio button for “Select archive file”.</li>

 <li>Browse to the zip file you downloaded and click Finish.</li>

</ol>

<strong> </strong>

<h1>More about grading</h1>




This is a “regular” assignment so we are going to read your code.  Your score will be based partly (about a third) on functional tests that we run and partly on the grader’s assessment of the quality of your code. Are you doing things in a simple and direct way that makes sense?  Are you defining redundant instance variables?  Some specific criteria that are important for this assignment are:




<ul>

 <li>Use instance variables only for the “permanent” state of the object, use local variables for temporary calculations within methods.</li>

</ul>

o You will lose points for having lots of unnecessary instance variables o All instance variables should be <strong><sub>private</sub></strong>.

<ul>

 <li><strong>Accessor methods should not modify instance variables</strong>.</li>

 <li>Avoid code duplication.</li>

 <li>Internal (//-style) comments are normally used inside of method bodies to explain <em>how</em> something works, while the Javadoc comments explain <em>what</em> a method does. Use internal comments where appropriate to explain how your code works. (A good rule of thumb is:</li>

</ul>

if you had to think for a few minutes to figure out how something works, you should probably include a comment explaining how it works.)

See the “Style and documentation” section below for additional guidelines.




<h1>Style and documentation</h1>




Roughly 15% of the points will be for documentation and code style.  Here are some general requirements and guidelines:

<ul>

 <li>Each class, method, constructor and instance variable, whether public or private, must have a meaningful and complete Javadoc comment. Class javadoc must include the</li>

</ul>

<strong>@author</strong> tag, and method javadoc must include <strong><sub>@param</sub></strong> and <strong><sub>@return</sub></strong> tags as appropriate.   o Try to state what each method does in your own words, but there is no rule against copying and pasting the descriptions from this document. o Run the javadoc tool and see what your documentation looks like! You do not have to turn in the generated html, but at least it provides some satisfaction &#x1f642;




<ul>

 <li>All variable names must be meaningful (i.e., named for the value they store). Your code should not be producing console output. You may add <strong><sub>println</sub></strong> statements when debugging, but you need to remove them before submitting the code.</li>

 <li>Try not to embed numeric literals in your code. Use the defined constants wherever appropriate.</li>

 <li>Use a consistent style for indentation and formatting.</li>

</ul>

o    Note that you can set up Eclipse with the formatting style you prefer and then use Ctrl-Shift-F to format your code.  To play with the formatting preferences, go to Window-&gt;Preferences-&gt;Java&gt;Code Style-&gt;Formatter and click the New button to create your own “profile” for formatting.

<strong> </strong>

<h1>If you have questions</h1>




For questions, please see the Piazza Q &amp; A pages and click on the folder <strong><sub>assignment3</sub></strong>. If you don’t find your question answered, then create a new post with your question.  Try to state the question or topic clearly in the title of your post, and attach the tag <strong><sub>assignment3</sub></strong>.  <em>But remember, do not post any source code for the classes that are to be turned in.</em> It is fine to post source code for general Java examples that are not being turned in, and <strong>for this assignment you are welcome to post and discuss test code</strong>.  (In the Piazza editor, use the button labeled “code” to have the editor keep your code formatting.  You can also use “pre” for short code snippets.)

<strong> </strong>

If you have a question that absolutely cannot be asked without showing part of your source code, change the visibility of the post to “private” so that only the instructors and TAs can see it.  Be sure you have stated a specific question; vague requests of the form “read all my code and tell me what’s wrong with it” will generally be ignored.




Of course, the instructors and TAs are always available to help you.  See the Office Hours section of the syllabus to find a time that is convenient for you.  We do our best to answer every question carefully, short of actually writing your code for you, but it would be unfair for the staff to fully review your assignment in detail before it is turned in.




Any posts from the instructors on Piazza that are labeled “Official Clarification” are considered to be part of the spec, and you may lose points if you ignore them.  Such posts will always be placed in the Announcements section of the course page in addition to the Q&amp;A page.  (We promise that no official clarifications will be posted within 24 hours of the due date.)

<strong> </strong>




<h1>What to turn in</h1>




<strong>Note: You will need to complete the “Academic Dishonesty policy questionnaire,” found on the Homework page on Canvas, before the submission link will be visible to you. </strong>




Please submit, on Canvas, the zip file that is created by the SpecChecker. The file will be named

<strong>SUBMIT_THIS_hw</strong><strong><sub>3.zip</sub></strong>. and it will be located in the directory you selected when you ran the SpecChecker.  It should contain one directory, <strong><sub>hw3</sub></strong>, which in turn contains two files, <strong><sub>Maze.java</sub></strong>, <strong>MazeCell</strong><strong><sub>.java</sub></strong>. Please LOOK at the file you upload and make sure it is the right one!




Submit the zip file to Canvas using the Assignment 1 submission link and verify that your submission was successful.  If you are not sure how to do this, see the document “Assignment Submission HOWTO” which can be found in the Piazza pinned messages.




We recommend that you submit the zip file as created by the specchecker.  If necessary for some reason, you can create a zip file yourself.  The zip file must contain the directory <strong>hw3</strong>, which in turn should contain two java files.  You can accomplish this by zipping up the <strong>src</strong> directory of your project.  The file must be a zip file, so be sure you are using the Windows or Mac zip utility, and NOT a third-party installation of WinRAR, 7-zip, or Winzip.

<strong> </strong>