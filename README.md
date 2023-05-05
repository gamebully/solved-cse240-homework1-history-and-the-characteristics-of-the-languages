Download Link: https://assignmentchef.com/product/solved-cse240-homework1-history-and-the-characteristics-of-the-languages
<br>
The aim of this assignment is to make sure that you understand and are familiar with the concepts covered in the lectures, including Unix operating system, programming paradigms, the structure of programming languages, and the differences between a macro and a procedure.  By the end of the assignment, you should have

<ul>

 <li>Learned a brief history of programming languages and the characteristics of the languages.</li>

 <li>Gotten started with Unix and GNU GCC the programming environment.</li>

</ul>




This assignment is related to the outcomes 1-2 and 1-3 listed in the syllabus:

<ul>

 <li>Students will understand the control structures of functional, logic, and imperative programming languages.</li>

 <li>Students will understand the execution of functional, logic, and imperative programming languages.</li>

</ul>

<strong>Reading</strong>: Read chapter 1, chapter 2 (sections 2.1, 2.2, and 2.3), appendix (sections B.1 and B.2), and course notes (slides).

You are expected to do the assignment outside the class meetings.   Should you need assistance, or have questions about the assignment, please contact the instructor or the TA during their Zoom office hours.

You are encouraged to ask and answer questions on the course discussion board.  (However, <strong>do not share your answers or code</strong> in the course discussion board.)







<h1>Pre-requisite</h1>

You are required to do these exercises, in order for you to do the following assignments that require submission.

<ol>

 <li>Subscribe to the General UNIX Cluster Server. You need to visit the ASU Computer Accounts Self-Sub website:</li>

</ol>

<a href="http://www.asu.edu/selfsub">http://www.asu.edu/selfsu</a><a href="http://www.asu.edu/selfsub">b</a><a href="http://www.asu.edu/selfsub">  </a>

You can login using your ASUAD User ID &amp; password. It will list your current subscriptions and what other options are available for you to subscribe. Add ASU <strong>General</strong> Computing Server if you don’t have it.

Your new General UNIX account may be ready immediately or may take a few days to become available. You can then log onto the “general.asu.edu” server using your ASUAD User ID and your password.

You need a secure telnet client like PuTTY or SSH to access the general server. You will use ASU General account and PuTTY or SSH for C/C++ and Prolog programming in this course. You can also create your personal web page in the folder called www in ASU General server.

In this course, you will use GNU gcc compiler to run C programs. Later in the semester, you will be required to use GNU Prolog under the General server to run all your Prolog programs. The course is designed to give you experience of using different kinds of programming environments!

<ol start="2">

 <li>Getting Started with GNU GCC on Unix</li>

</ol>

To do the C assignments using GNU GCC, you need to have basic Unix knowledge. If you are not familiar with basic Unix commands, you need to read textbook Appendix B, sections B.1 and B.2.1 and the Unix Tutorial given in the homework folder.

In order to connect to ASU general server, you need to install and use ASU VPN:

Enter MyASU –&gt; My Apps –&gt; Search VPN

You will find: <a href="https://webapp3.asu.edu/myapps/Search/0/VPN#quicklinkContainer1139"> </a><a href="https://webapp3.asu.edu/myapps/Search/0/VPN#quicklinkContainer1139">Cisco Anyconnect SSLVPN.</a> Install and enter the connection address: sslvpn.asu.edu. Then, you can use your ASUAD account to connect.

Once you have connected your sslvpn, you can connect to ASU General. Enter the “general.asu.edu” server by using PuTTY or SHH to connect to <em>general.asu.edu</em>.

<ul>

 <li><em>If you already have an account on </em>General<em>, then skip ahead to the next exercise</em>. Otherwise, in your browser, navigate to <a href="http://www.asu.edu/selfsub">http://www.asu.edu/selfsu</a><a href="http://www.asu.edu/selfsub">b</a> <a href="http://www.asu.edu/selfsub">an</a>d subscribe to <strong>asu.edu </strong>to obtain an account on that system. It takes anywhere from a few minutes to perhaps an hour for your account to be activated. Please read Unix Tutorial for more detail.</li>

 <li>Once your account is activated, run a <strong>secure shell terminal</strong> program such as <strong>PuTTY </strong>or <strong>SSH</strong> on your PC or Mac. Configure the terminal program to connect to <strong>asu.edu</strong> (in the <strong>host name </strong>text field) on <strong>port 22</strong>.</li>

</ul>




<ul>

 <li>Log in to <strong>General </strong>using your ASUAD</li>

 <li>Do a <strong>pwd</strong> command to determine your home directory. What is the <strong>absolute</strong> path name of your home directory?</li>

</ul>

For example, when I log in to <strong>General </strong>and perform a <strong>pwd</strong> command, I see,

/afs/asu.edu/users/y/c/h/ychen1

Of course, it should be the path from the root to your directory.

<ul>

 <li>Do an <strong>ls</strong> command to see the files in your home directory.</li>

 <li>Do an <strong>ls -a</strong> command to see <strong>all </strong>of the files in your home directory, including hidden files.</li>

 <li>Do an <strong>ls -l</strong> command to produce a <strong>long </strong>listing of the non-hidden files in your home directory.</li>

 <li>Do an <strong>ls -al</strong> command to produce a <strong>long </strong>listing of <strong>all </strong>of the files in your home directory.</li>

</ul>

Make a new directory (e.g. MyDir or CSE240) by using the command: <em>mkdir MyDir</em>, use this to store all of your C and C++ programs in a specific directory. You may create subdirectories in this directory.

Enter the directory by using Change Directory command: <em>cd MyDir</em>

Please note that you can remotely connect (using PuTTY or SSH) to the general server from anywhere, at any time, that is, you can do the assignment at home.

To write a GNU GCC program on a Unix server, you can either use a Unix editor, e.g., <em>vim</em> or <em>pico</em> or upload (using the same PuTTY software that includes SSH/telnet) a pre-edited file into your Unix directory <em>MyDir</em>. The name of a C program should have an extension .<em>c</em> and the name of a C++ program should have an extension .<em>cpp </em>

<strong> </strong>

<strong> </strong>

<h1>Programming Exercise (50 points)</h1>

<ol>

 <li>Follow the Textbook Appendix B and the Unix Tutorial PPT given in the homework folder to complete the following tasks:

  <ul>

   <li>Create a new directory called CSE240. Use cd CSE240 to enter the new directory. Use pwd command to find the path from the Unix root directory to your current directory.</li>

   <li>Create three new subdirectories inside CSE240. Name the directories d1, d2, and d3 respectively.</li>

   <li>Enter the directory d1 and use vi or vim to create a new program called hello.c and enter the following code into the program. You must use your name to replace the name “John Doe”. Save the file.</li>

  </ul></li>

</ol>




Use <em>gcc hello.c -o hello</em> to compile the program. Fix any compilation errors if any.

<ul>

 <li>Use ls, ls -l, and ls -al respectively to list files in d1 directory. Use command ./hello to execute the compiled code. .    [4 points]</li>

</ul>

Take screenshots of each command in this question. You may take one screenshot with all commands in it.

<ul>

 <li>Enter d2 directory and then use one command to copy (not move) the files hello.c and hello from d1 directory into d2 directory. Use ls -al to view all the files in d2.</li>

</ul>

Take screenshots of each command in this question. You may take one screenshot with all commands in it.           [3 points]

<ul>

 <li>In d2 directory, use chmod 660 hello to change the permission. Use ls -l to view the files. Use command ./hello to execute the compiled code. Take a screenshot of this output. Use chmod command again to make hello an executable, but not readable and not writeable for all users. Use command ./hello to execute the compiled code.</li>

</ul>

Take a  screenshot of this output.                                                                [4 points]

<ul>

 <li>Enter CSE240 directory. Use ls -l to view all the files. Then, use one command to delete d2 directory and all the files in d2 directory. Use ls -l to view all the files.</li>

</ul>

Take screenshots of each command in this question. You may take one screenshot with all commands in it.           [3 points]

Screenshots needed for questions 1.4 through 1.7. Put all the screenshots along with their question numbers in a word file and convert to pdf. Submit the file as hw01q1.pdf

<ol start="2">

 <li>In this question, you will use Unix tools to edit, debug, and execute a simple C program. The purpose of the homework is to learn the Unix programming environment. Read textbook Section 2.2.3, the tutorials, and the Unix tutorial in text Appendix B.2.

  <ul>

   <li>Use a text editor to enter the following program. Variations and more discussions of this program can be found in textbook Section 2.1.3. Use GNU GCC to compile, debug (find and fix any syntax errors), and execute the program and fix any semantic errors, for example, by adding “break” statements in the required places and by fixing incorrect characters copied into the programming environment, if any, and by type-changing to print a floating point number. The code is supposed to perform one math operation in each switch-case. The ‘ch’ variable is assigned a new math operator before each switch-case. Submit the corrected program as hw01q2.c [8 points]</li>

  </ul></li>

</ol>




<table width="587">

 <tbody>

  <tr>

   <td width="587">/* This C program demonstrates the switch statement without using breaks. */#include &lt;stdio.h&gt;   main() {char ch = ‘+’;int a = 10, b = 20;double f;printf(“ch = %c
”, ch);switch (ch) {case ‘+’: f = a + b; printf(“f = %d
”, f);          case ‘-‘: f = a – b; printf(“f = %d
”, f);          case ‘*’: f = a * b; printf(“f = %d
”, f);          case ‘/’: f = a / b; printf(“f = %d
”, f);          default: printf(“invalid operator
”);}ch = ‘-‘;printf(“ch = %c
”, ch);switch (ch) {case ‘+’: f = a + b; printf(“f = %d
”, f);          case ‘-‘: f = a – b; printf(“f = %d
”, f);          case ‘*’: f = a * b; printf(“f = %d
”, f);          case ‘/’: f = a / b; printf(“f = %d
”, f);          default: printf(“invalid operator
”);}ch = ‘*’;printf(“ch = %c
”, ch);switch (ch) {case ‘+’: f = a + b; printf(“f = %d
”, f);          case ‘-‘: f = a – b; printf(“f = %d
”, f);</td>

  </tr>

  <tr>

   <td width="587"><sub> </sub>            case ‘*’: f = a * b; printf(“f = %d
”, f);case ‘/’: f = a / b; printf(“f = %d
”, f);<sup> </sup><sup>            </sup>default: printf(“invalid operator
”);} ch =<sup> </sup><sup>         </sup>‘/’printf(;  “ch = %c
”, ch);             switch (ch) {case ‘+’: f = a + b; printf(“f = %d
”, f); case ‘-‘: f = a – b; printf(“f = %d
”, f);              case ‘*’: f = a * b; printf(“f = %d
”, f); <sub> </sub>            case ‘/’: f = a / b; printf(“f = %d
”, f); default: printf(“invalid operator
”);<sup> </sup><sup>            </sup>} ch =‘%’;<sub>  </sub>printf(switch “ch = %c(ch) {  
”, ch);case ‘+’: f = a + b; printf(“f = %d
”, f);             case ‘-‘: f = a – b; printf(“f = %d
”, f); case ‘*’: f = a * b; printf(“f = %d
”, f); <sup> </sup><sup>            </sup>case ‘/’: f = a / b; printf(“f = %d
”, f);             default: printf(“invalid operator
”); }}</td>

  </tr>

 </tbody>

</table>




<ul>

 <li>Edit the code above or write a new code to use a for-loop (that runs 5 times) to ask the user for a math operation as input ( +, – , * , / ). Use an input statement such as <em>ch = getchar();</em> or <em>scanf(“%c
”, &amp;ch);</em> to replace the assignment statement <em>ch = </em><em>‘+’ </em>in the code above. Expected result shown in the figure below. Submit the revised</li>

</ul>

program as hw01q2_2.c.                                                                                   [8 points]




Note, when you add the loop, you may need to use a <em>fflush(stdin)</em> or a <em>getchar()</em> to flush the newline ‘
’ character left behind by a previous operation; You can use one ch = getchar() at the beginning of the loop and one before the end of the loop:  for ( … )

{

printf(“please enter a char”); ch = getchar(); // read a char

other code;      ch = getchar(); // This line will flush ‘
’ character left behind by the previous getchar().

ch = getchar(); // You may need this one to keep the console window open

}

Please read text Section 2.1.3 for more details.

<ol start="3">

 <li>You are given a file named “hw01q3.c”. All instructions are given in the form of comments in the file. You should correct the errors and identify which error type they are. Please read all instructions carefully, then complete and submit the updated file</li>

</ol>


