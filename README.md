
<!DOCTYPE html>
<html>
 <head>
  <meta charset="utf-8">
   <title>
    Problem Set 0: Turtle Graphics
   </title>
   <link href="../../web/handout-style.css" rel="stylesheet">
    <meta content="width=device-width, initial-scale=1" name="viewport"/>
   </link>
  </meta>
 </head>
 <body>
  <header>
   <a href="https://ocw.mit.edu/ans7870/6/6.005/s16/">
    6.005 — Software Construction on MIT OpenCourseWare
   </a>
   |
   <a href="https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-005-software-construction-spring-2016/">
    OCW 6.005 Homepage
   </a>
   <div>
    Spring 2016
   </div>
  </header>
  <nav class="table-of-contents col-sm-2">
   <ul class="nav">
    <li>
     <a href="#problem_set_0_turtle_graphics">
      Problem Set 0: Turtle Graphics
     </a>
    </li>
    <li>
     <a href="#part_i">
      Part I
     </a>
    </li>
    <li>
     <a href="#problem_0_install_and_set_up">
      Problem 0: Install and set up
     </a>
    </li>
    <li>
     <a href="#clone">
      Problem 1: Clone and import
     </a>
    </li>
    <li>
     <a href="#problem_2_warm_up_with_mayusecodeinassignment">
      Problem 2: Warm up with may­Use­Code­In­Assignment
     </a>
    </li>
    <li>
     <a href="#unit_testing">
      Unit testing
     </a>
    </li>
    <li>
     <a href="#problem_3_commit_and_push_rulesof6005">
      Problem 3: Commit and push Rules­Of­6005
     </a>
    </li>
    <li>
     <a href="#part_ii">
      Part II
     </a>
    </li>
    <li>
     <a href="#turtle_graphics_and_the_logo_language">
      Turtle graphics and the Logo language
     </a>
    </li>
    <li>
     <a href="#problem_4_drawsquare">
      Problem 4: drawSquare
     </a>
    </li>
    <li>
     <a href="#problems_510_polygons_and_headings">
      Problems 5—10: Polygons and headings
     </a>
    </li>
    <li>
     <a href="#problem_11_personal_art">
      Problem 11: Personal art
     </a>
    </li>
   </ul>
  </nav>
  <main class="container-fluid">
   <h1 class="handout-title col-sm-8 col-sm-offset-2" id="problem_set_0_turtle_graphics">
    Problem Set 0: Turtle Graphics
   </h1>
   <div data-outline="problem_set_0_turtle_graphics">
    <div class="markdown col-sm-8 col-sm-offset-2 converted">
     <p>
      <strong>
       Welcome to 6.005!
      </strong>
     </p>
     <p>
      This course is about three essential properties of software:
     </p>
     <table class="table table-striped no-markdown">
      <tbody>
       <tr>
        <th width="33%">
         Safe from bugs
        </th>
        <th>
         Easy to understand
        </th>
        <th>
         Ready for change
        </th>
       </tr>
       <tr>
        <td>
         Correct today and correct in the unknown future.
        </td>
        <td>
         Communicating clearly with future programmers, including future you.
        </td>
        <td>
         Designed to accommodate change without rewriting.
        </td>
       </tr>
      </tbody>
     </table>
     <p>
      The purpose of this problem set is to:
     </p>
     <ul>
      <li>
       introduce the tools we will use in 6.005, including Java, Eclipse, JUnit, and Git;
      </li>
      <li>
       introduce the process for 6.005 problem sets;
      </li>
      <li>
       and practice basic Java and start using tools from the Java standard library.
      </li>
     </ul>
     <p>
      You should focus in this problem set on writing code that is
      <strong>
       safe from bugs
      </strong>
      and
      <strong>
       easy to understand
      </strong>
      using the techniques we discuss in class.
     </p>
     <hr>
      <h1 id="part_i">
       Part I
      </h1>
      <div data-outline="part_i">
       <h2 id="problem_0_install_and_set_up">
        Problem 0: Install and set up
       </h2>
       <div data-outline="problem_0_install_and_set_up">
        <div class="handout-solo alert alert-warning">
         <p>
          Read and complete the
          <a class="alert-link" href="../../getting-started/">
           <strong>
            Getting Started guide
           </strong>
          </a>
          .
The guide will step through:
         </p>
         <ul>
          <li>
           installing the JDK, Eclipse, and Git
          </li>
          <li>
           configuring Eclipse
          </li>
          <li>
           configuring Git
          </li>
          <li>
           learning and practicing the basics of Git
          </li>
         </ul>
        </div>
        <p>
         You need to complete all the steps in the guide before you start working on this problem set.
        </p>
       </div>
       <h2 id="clone">
        Problem 1: Initialize the Git Repo
       </h2>
       <div data-outline="clone">
        <p>
         This process will be identical for each problem set.
        </p>
        <ol>
         <li>
          <p>
           <strong>
            Initialize your repo.
           </strong>
           <p>
            Download the project code
            <a href="ps0.zip">
             here
            </a>
            . In the terminal, navigate to the folder containing the project code and run:
           </p>
           <blockquote class="no-markdown pull-margin">
            <tt>
             git init
            </tt>
           </blockquote>
           <li>
            <span id="import">
            </span>
            <p>
             After cloning your repository,
             <strong>
              add the project to Eclipse
             </strong>
             so you can work on it.
            </p>
            <p>
             Note:
             <a href="../../getting-started/#config-eclipse">
              Getting Started step 2
             </a>
             has setup you must perform before using Eclipse in 6.005.
            </p>
            <p>
             <strong>
              To import a project:
             </strong>
            </p>
            <ul>
             <li>
              In Eclipse, go to
              <em>
               File → Import… → Git → Projects from Git
              </em>
             </li>
             <li>
              On the “Select Repository Source” page, select “Existing local repository”
             </li>
             <li>
              On “Select a Git Repository,” click Add…, and Browse… to the directory of your clone
             </li>
             <li>
              The “Search results” list should show your clone, with “.git” at the end; click “Finish”
             </li>
             <li>
              On “Select a wizard” for importing, choose “Import existing projects”
             </li>
             <li>
              Finally, on “Import projects,” make sure ps0 is checked, and click “Finish”
             </li>
            </ul>
           </li>
          </p>
         </li>
        </ol>
       </div>
       <h2 id="problem_2_warm_up_with_mayusecodeinassignment">
        Problem 2: Warm up with
        <code>
         may­Use­Code­In­Assignment
        </code>
       </h2>
       <div data-outline="problem_2_warm_up_with_mayusecodeinassignment">
        <div class="list-style-lower-alpha">
         <ol>
          <li>
           <p>
            Look at the source code contained in
            <code>
             RulesOf6005.java
            </code>
            in package
            <code>
             rules
            </code>
            .
Your warm-up task is to implement:
           </p>
           <pre><code class="language-java hljs">mayUseCodeInAssignment(
       <span class="hljs-keyword">boolean</span> writtenByYourself, <span class="hljs-keyword">boolean</span> availableToOthers,
       <span class="hljs-keyword">boolean</span> writtenAsCourseWork, <span class="hljs-keyword">boolean</span> citingYourSource,
       <span class="hljs-keyword">boolean</span> implementationRequired)</code></pre>
           <p>
            You can find the policy under
            <a href="../../general/">
             General Information
            </a>
            on the
            <a href="../../">
             course home page
            </a>
            .
           </p>
          </li>
          <li>
           <p>
            Once you’ve implemented this method, run the
            <code>
             main
            </code>
            method in
            <code>
             RulesOf6005.java
            </code>
            .
           </p>
           <p>
            <code>
             public static void main(String[] args)
            </code>
            is the entry point for Java programs.
In this case, the
            <code>
             main
            </code>
            method calls the
            <code>
             mayUseCodeInAssignment
            </code>
            method with input parameters.
To run
            <code>
             main
            </code>
            in
            <code>
             RulesOf6005
            </code>
            , right click on the file
            <code>
             RulesOf6005.java
            </code>
            in either your Package Explorer, Project View, or Navigator View, go to the
            <em>
             Run As
            </em>
            option, and click on
            <em>
             Java Application
            </em>
            .
           </p>
          </li>
         </ol>
        </div>
        <div class="panel panel-default">
         <div class="panel-body">
          <h2 id="unit_testing">
           Unit testing
          </h2>
          <div data-outline="unit_testing">
           <p>
            Right now, we can use the
            <code>
             main
            </code>
            method plus some visual inspection to verify that our implementation is correct.
More generally, programs will have many dozens of methods that need to be tested; visually inspecting output for each one is fragile, time-consuming, and inherently non-scalable.
           </p>
           <p>
            Instead, we will use
            <em>
             automated unit testing
            </em>
            , which runs a suite of tests to automatically test whether the implementations are correct. 
For this problem set, we will write unit tests for methods that do not draw graphics on the screen; unit-testing GUIs is a more complex problem.
           </p>
           <h3 id="automated_unit_testing_with_junit">
            Automated unit testing with JUnit
           </h3>
           <div data-outline="automated_unit_testing_with_junit">
            <p>
             <a href="//www.junit.org/">
              JUnit
             </a>
             is a widely-adopted Java unit testing library, and we will use it heavily in 6.005.
A major component of the 6.005 design philosophy is to decompose problems into minimal, orthogonal units, which can be assembled into the larger modules that form the finished program.
One benefit of this approach is that each unit can be tested thoroughly, independently of others, so that faults can be quickly isolated and corrected as code is rewritten and modules are configured.
Unit testing is the technique of writing tests for the smallest testable pieces of functionality, to allow for the flexible and organic evolution of complex, correct systems.
            </p>
            <p>
             By writing thoughtful unit tests, it is possible to verify the correctness of one’s code, and to be confident that the resulting programs behave as expected.
In 6.005, we will use JUnit version 4.
            </p>
           </div>
           <h3 id="anatomy_of_junit">
            Anatomy of JUnit
           </h3>
           <div data-outline="anatomy_of_junit">
            <p>
             JUnit unit tests are written method by method.
There is nothing special a class has to do to be used by JUnit; it only need contain methods that JUnit knows to call, which we call
             <em>
              test methods
             </em>
             .
Test methods are specified using
             <em>
              annotations
             </em>
             , which may be thought of as keywords (more specifically, they are a type of metadata), that can be attached to individual methods and classes.
Though they do not themselves change the meaning of a Java program, at compile- or run-time other code can detect the annotations and make decisions accordingly.
Though we will not deeply explore annotations in 6.005, you will see a few important uses of them.
            </p>
            <p>
             Look closely at
             <code>
              RulesOf6005Test.java
             </code>
             , and note the
             <code>
              @Test
             </code>
             that precedes method definitions.
This is an example of an annotation.
The JUnit library uses this annotation to determine which methods to call when running unit tests.
The
             <code>
              @Test
             </code>
             annotation denotes a test method; there can be any number in a single class.
Even if one test method fails, the others will be run.
            </p>
            <p>
             Unit test methods can contain calls to
             <code>
              assertEquals
             </code>
             , which is an assertion that compares two objects against each other and fails if they are not equal,
             <code>
              assertTrue
             </code>
             , which checks if the condition is true, and
             <code>
              assertFalse
             </code>
             , which checks if the condition is false.
             <a href="//junit.org/javadoc/latest/index.html?org/junit/Assert.html">
              Here is a list of all the assertions supported by JUnit
             </a>
             .
If an assertion in a test method fails, that test method returns immediately, and JUnit records a failure for that test.
            </p>
           </div>
          </div>
         </div>
        </div>
        <div class="list-style-lower-alpha">
         <ol start="3">
          <li>
           <p>
            Run the unit tests.
           </p>
           <p>
            To run the tests in
            <code>
             RulesOf6005Test
            </code>
            , right click on the
            <code>
             RulesOf6005Test.java
            </code>
            file in either your Package Explorer, Project View, or Navigator View, and go to the
            <em>
             Run As
            </em>
            option.
Click on
            <em>
             JUnit Test
            </em>
            , and you should see the JUnit view appear.
           </p>
           <p>
            If your implementation of
            <code>
             mayUseCodeInAssignment
            </code>
            is correct, you should see a green bar, indicating that all the tests (there’s only 1 test, containing 2 assertions) passed.
           </p>
          </li>
          <li>
           <p>
            Try
            <em>
             breaking
            </em>
            your implementation and running
            <code>
             RulesOf6005Test
            </code>
            again.
           </p>
           <p>
            You should see a red bar in the JUnit view, and if you click on
            <code>
             test­May­Use­Code­In­Assignment
            </code>
            , you will see a
            <em>
             stack trace
            </em>
            in the bottom box, which provides a brief explanation of what went wrong.
Double-clicking on a line in the failure stack trace will bring up the code for that frame in the trace.
This is most useful for lines that correspond to your code; this stack trace will also contain lines for Java libraries or JUnit itself.
           </p>
          </li>
          <li>
           <p>
            Enough breaking: fix your implementation so it’s correct again.
Make sure the tests pass.
           </p>
           <p>
            Passing the JUnit tests we provide does
            <strong>
             not
            </strong>
            necessarily mean that your code is perfect.
You need to review the function specifications carefully, and
            <strong>
             always write your own JUnit tests
            </strong>
            to verify your code.
           </p>
          </li>
         </ol>
        </div>
       </div>
       <h2 id="problem_3_commit_and_push_rulesof6005">
        Problem 3: Commit and push
        <code>
         Rules­Of­6005
        </code>
       </h2>
       <div data-outline="problem_3_commit_and_push_rulesof6005">
        <p>
         After you’ve finished implementing the function and verified that it is correct, let’s do a first commit.
        </p>
        <ol>
         <li>
          <p>
           First, in the terminal, change directory (
           <code>
            cd
           </code>
           ) to your clone, and take a look around with
          </p>
          <blockquote>
           <p>
            <code>
             git status
            </code>
           </p>
          </blockquote>
          <p>
           which shows you files that have been created, deleted, and modified in the project directory.
You should see
           <code>
            RulesOf6005.java
           </code>
           listed under “Changes not staged for commit.”
This means Git sees the change, but you have not (yet) asked Git to include the change as part of your next commit.
          </p>
         </li>
         <li>
          <p>
           You can run the command
          </p>
          <blockquote>
           <p>
            <code>
             git diff
            </code>
           </p>
          </blockquote>
          <p>
           to see your changes.
(
           <strong>
            Note
           </strong>
           : when the diff is more than one page long, use the arrow keys.
Press
           <code>
            q
           </code>
           to quit the diff.)
          </p>
         </li>
         <li>
          <p>
           Before committing, files must be
           <em>
            staged
           </em>
           for commit.
Staging a file is as simple as
          </p>
          <blockquote>
           <p>
            <code>
             git add &lt;filename&gt;
            </code>
           </p>
          </blockquote>
          <p>
           so use
          </p>
          <blockquote>
           <p>
            <code>
             git add src/rules/RulesOf6005.java
            </code>
           </p>
          </blockquote>
          <p>
           to stage the file.
You should also stage the test file if you’ve added more tests.
          </p>
         </li>
         <li>
          <p>
           In addition, it’s always a good idea to review your commits before committing to them. Run
          </p>
          <blockquote>
           <p>
            <code>
             git status
            </code>
           </p>
          </blockquote>
          <p>
           again to see that your changes are now listed under “Changes to be committed.” If you run
          </p>
          <blockquote>
           <p>
            <code>
             git diff
            </code>
           </p>
          </blockquote>
          <p>
           those changes are no longer shown! Use
          </p>
          <blockquote>
           <p>
            <code>
             git diff --staged
            </code>
           </p>
          </blockquote>
          <p>
           to see exactly what Git will record if you commit now.
          </p>
         </li>
         <li>
          <p>
           Ready? To perform the commit,
          </p>
          <blockquote>
           <p>
            <code>
             git commit
            </code>
           </p>
          </blockquote>
          <p>
           will actually commit the changes locally, after opening your default editor to allow you to write a commit message.
Your message should be formatted according to the
           <a href="//git-scm.com/book/ch5-2.html#Commit-Guidelines">
            Git standard
           </a>
           : a short summary that fits on one line, followed by a blank line and a longer description if necessary.
          </p>
          <p>
           <strong>
            If Git warns you about configuring your default identity or you can’t edit your commit message
           </strong>
           , you did not follow the instructions in the Getting Started guide.
           <a href="../../getting-started/#config-git">
            Getting Started step 5
           </a>
           has setup you must perform before using Git.
          </p>
          <p>
           Now run
          </p>
          <blockquote>
           <p>
            <code>
             git status
            </code>
           </p>
          </blockquote>
          <p>
           once more, and see that your changes are no longer listed.
          </p>
         </li>
         <li>
          <p>
           You can use the command
          </p>
          <blockquote>
           <p>
            <code>
             git log
            </code>
           </p>
          </blockquote>
          <p>
           to see the history of commits in your project.
Right now, you should see two of them: the initial commit to create your problem set repository with the starting code, and the commit you made just now.
          </p>
          <p>
           <strong>
            Important:
           </strong>
           only the local history has the new commit at this point; it is not stored in your remote repository.
This is one important aspect where Git is different from centralized systems such as Subversion and CVS.
          </p>
         </li>
         <hr/>
        </ol>
       </div>
      </div>
      <h1 id="part_ii">
       Part II
      </h1>
      <div data-outline="part_ii">
       <h2 id="turtle_graphics_and_the_logo_language">
        Turtle graphics and the Logo language
       </h2>
       <div data-outline="turtle_graphics_and_the_logo_language">
        <p>
         <a href="//en.wikipedia.org/wiki/Logo_%28programming_language%29">
          Logo
         </a>
         is a programming language created at MIT that originally was used to move a robot around in space.
Turtle graphics, added to the Logo language, allows programmers to issue a series of commands to an on-screen “turtle” that moves, drawing a line as it goes.
Turtle graphics have also been added to many different programming languages,
         <a href="//docs.python.org/2/library/turtle.html">
          including Python
         </a>
         , where it is part of the standard library.
        </p>
        <p>
         In the rest of problem set 0, we will be playing with a simple version of turtle graphics for Java that contains a restricted subset of the Logo language:
        </p>
        <ul>
         <li>
          <code>
           forward(units)
          </code>
          <br>
           Moves the turtle in the current direction by
           <em>
            units
           </em>
           pixels, where units is an integer.
Following the original Logo convention, the turtle starts out facing up.
          </br>
         </li>
         <li>
          <code>
           turn(degrees)
          </code>
          <br>
           Rotates the turtle by angle
           <em>
            degrees
           </em>
           to the right (clockwise), where degrees is a double precision floating point number.
          </br>
         </li>
        </ul>
        <p>
         You can see the definitions of these commands in
         <code>
          Turtle.java
         </code>
         .
        </p>
        <p>
         <strong>
          Do NOT use any turtle commands other than
          <code>
           forward
          </code>
          and
          <code>
           turn
          </code>
          in your code for the following methods.
         </strong>
        </p>
       </div>
       <h2 id="problem_4_drawsquare">
        Problem 4:
        <code>
         drawSquare
        </code>
       </h2>
       <div data-outline="problem_4_drawsquare">
        <p>
         Look at the source code contained in
         <code>
          TurtleSoup.java
         </code>
         in package
         <code>
          turtle
         </code>
         .
        </p>
        <p>
         Your task is to implement
         <code>
          drawSquare(Turtle turtle, int sideLength)
         </code>
         , using the two methods introduced above:
         <code>
          forward
         </code>
         and
         <code>
          turn
         </code>
         .
        </p>
        <p>
         Once you’ve implemented the method, run the
         <code>
          main
         </code>
         method in
         <code>
          TurtleSoup.java
         </code>
         .
The
         <code>
          main
         </code>
         method in this case simply creates a new turtle, calls your
         <code>
          drawSquare
         </code>
         method, and instructs the turtle to draw.
Run the method by going to
         <em>
          Run → Run As… → Java Application
         </em>
         .
A window will pop up, and, once you click the “Run!” button, you should see a square drawn on the canvas.
        </p>
       </div>
       <h2 id="problems_510_polygons_and_headings">
        Problems 5—10: Polygons and headings
       </h2>
       <div data-outline="problems_510_polygons_and_headings">
        <p>
         <strong>
          For detailed requirements, read the specifications of each function to be implemented above its declaration in
          <code>
           TurtleSoup.java
          </code>
          .
Be careful when dealing with mixed integer and floating point calculations.
         </strong>
        </p>
        <p>
         You should not change any of the
         <em>
          method declarations
         </em>
         (
         <a href="//docs.oracle.com/javase/tutorial/java/javaOO/methods.html">
          what’s a declaration?
         </a>
         ) below.
If you do so, you risk receiving
         <strong>
          zero points
         </strong>
         on the problem set.
        </p>
        <h3 id="drawing_polygons">
         Drawing polygons
        </h3>
        <div data-outline="drawing_polygons">
         <ul>
          <li>
           <p>
            Implement
            <code>
             calculateRegularPolygonAngle
            </code>
            <br>
             There’s a simple formula for what the inside angles of a regular polygon should be; try to derive it before googling/binging/duckduckgoing.
            </br>
           </p>
          </li>
          <li>
           <p>
            Run the JUnit tests in
            <code>
             TurtleSoupTest
            </code>
            <br>
             The method that tests
             <code>
              calculateRegularPolygonAngle
             </code>
             should now pass and show green instead of red.
            </br>
           </p>
           <p>
            If
            <code>
             testAssertionsEnabled
            </code>
            fails, you did not follow the instructions in the
Getting Started guide.
            <a href="../../getting-started/#config-eclipse">
             Getting Started step 2
            </a>
            has setup you must perform before using Eclipse.
           </p>
          </li>
          <li>
           <p>
            Implement
            <code>
             calculatePolygonSidesFromAngle
            </code>
            <br>
             This does the inverse of the last function; again, use the simple formula.
However,
             <strong>
              make sure you correctly round
             </strong>
             to the nearest integer.
Instead of implementing your own rounding, look at Java’s
             <a href="//docs.oracle.com/javase/8/docs/api/?java/lang/Math.html">
              <code>
               java.lang.Math
              </code>
             </a>
             class for the proper function to use.
            </br>
           </p>
          </li>
          <li>
           <p>
            Implement
            <code>
             drawRegularPolygon
            </code>
            <br>
             Use your implementation of
             <code>
              calculateRegularPolygonAngle
             </code>
             .
To test this, change the
             <code>
              main
             </code>
             method to call
             <code>
              drawRegularPolygon
             </code>
             and verify that you see what you expect.
            </br>
           </p>
          </li>
         </ul>
        </div>
        <h3 id="calculating_headings">
         Calculating headings
        </h3>
        <div data-outline="calculating_headings">
         <ul>
          <li>
           <p>
            Implement
            <code>
             calculateHeadingToPoint
            </code>
            <br>
             This function calculates the parameter to
             <code>
              turn
             </code>
             required to get from a current point to a target point, with the current direction as an additional parameter.
For example, if the turtle is at (0,1) facing 30 degrees, and must get to (0,0), it must turn an additional 150 degrees, so
             <code>
              calculateHeadingToPoint(30, 0, 1, 0, 0)
             </code>
             would return
             <code>
              150.0
             </code>
             .
            </br>
           </p>
          </li>
          <li>
           <p>
            Implement
            <code>
             calculateHeadings
            </code>
            <br>
             Make sure to use your
             <code>
              calculateHeadingToPoint
             </code>
             implementation here.
For information on how to use Java’s
             <code>
              List
             </code>
             interface and classes implementing it, look up
             <a href="//docs.oracle.com/javase/8/docs/api/?java/util/List.html">
              <code>
               java.util.List
              </code>
             </a>
             in the Java library documentation.
Note that for a list of
             <em>
              n
             </em>
             points, you will return
             <em>
              n-1
             </em>
             heading adjustments; this list of adjustments could be used to guide the turtle to each point in the list.
For example, if the input lists consisted of
             <code>
              xCoords=[0,0,1,1]
             </code>
             and
             <code>
              yCoords=[1,0,0,1]
             </code>
             (representing points (0,1), (0,0), (1,0), and (1,1)), the returned list would consist of
             <code>
              [180.0, 270.0, 270.0]
             </code>
             .
            </br>
           </p>
          </li>
         </ul>
        </div>
       </div>
       <h2 id="problem_11_personal_art">
        Problem 11: Personal art
       </h2>
       <div data-outline="problem_11_personal_art">
        <ul>
         <li>
          <p>
           Implement
           <code>
            drawPersonalArt
           </code>
           <br>
            In this function, you have the freedom to draw any piece of art you wish.
Your work will be judged both on aesthetics and on the code used to draw it.
Your art doesn’t need to be complex, but it should be more than a few lines.
Use helper methods, loops, etc. rather than simply listing forward and turn commands.
           </br>
          </p>
          <p>
           <strong>
            For
            <code>
             drawPersonalArt
            </code>
            only, you may also use the
            <code>
             color
            </code>
            method of
            <code>
             Turtle
            </code>
            to change the pen color.
           </strong>
           You may only use the provided colors.
          </p>
          <p>
           <a href="https://www.google.com/search?q=python+turtle+example+images">
            Here are some examples
           </a>
           of the kinds of images you can generate procedurally with turtle graphics, though note that many of them use more commands than what we’ve provided here.
Modify the
           <code>
            main
           </code>
           method to see the results of your function.
          </p>
         </li>
        </ul>
        <hr/>
       </div>
      </div>
     </hr>
    </div>
   </div>
  </main>
  <footer>
   MIT EECS
  </footer>
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.2.0/jquery.min.js" type="text/javascript">
  </script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/js/bootstrap.min.js" type="text/javascript">
  </script>
  <script src="../../web/handout-run.js" type="text/javascript">
  </script>
 </body>
</html>
<!-- Handout delivered Tue Feb 02 2016 00:50:12 GMT-0500 (EST) -->
