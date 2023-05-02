Download Link: https://assignmentchef.com/product/solved-comp2710-project-4-a-simple-trivia-quiz-game
<br>
<strong><em>  </em></strong>

<ul>

 <li>To learn how to use linked data structures (Note: no array is allowed)</li>

 <li>To use strings</li>

 <li>To learn creating multiple versions via conditional compilation</li>

 <li>To design and implement functions</li>

 <li>To perform unit testing</li>

</ul>




In this homework assignment, you will write a simple trivia quiz game. You program first allows players to create their trivia questions and answers. Multiple questions should be organized and managed using <strong><u>a linked data structure; no array is allowed in this</u> <u>homework assignment</u></strong>. Then, your program asks a question to the player, input the player’s answer, and check if the player’s answer matches the actual answer. If so, award the player the award points for that question. If the player enters the wrong answer your program should display the correct answer. When all questions have been asked display the total amount that the player has won.




Please perform the following steps to finish this assignment.

<ul>

 <li><strong>Step 1:</strong> Creating a TriviaNode <strong>structure</strong> that contains (1) information about a single trivia question and (2) a pointer pointing to other TriviaNode. This structure must contain a <strong>string</strong> for the question, a <strong>string</strong> for the answer to the question, an integer representing points the question is worth, and <strong>a pointer of the TriviaNode type</strong>. Please keep in mind that a harder question should be worth more points.</li>

 <li><strong>Step 2:</strong> Create a linked list of Trivia using the TriviaNode structure defined in Step 1.</li>

 <li><strong>Step 3:</strong> Design and implement a function that initialize the Trivia linked list by hard-coding the following three (3) trivia questions (including answers and award points). The o Trivia 1:

  <ul>

   <li>Question: How long was the shortest war on record? (Hint: how many minutes)</li>

   <li>Answer: 38</li>

   <li>Award points: 100 o Trivia 2:</li>

   <li>Question: What was Bank of America’s original name? (Hint: Bank of Italy or Bank of Germany)</li>

   <li>Answer: Bank of Italy</li>

   <li>Award points: 50 o Trivia 3:</li>

   <li>Question: What is the best-selling video game of all time? (Hint: Call of Duty or Wii Sports)?</li>

   <li>Answer: Wii Sports</li>

   <li>Award points: 20</li>

  </ul></li>

 <li><strong>Step 4:</strong> Design and implement a function to create and add a new TriviaNode into the linked list. You must use operator <strong>new</strong> to dynamic allocate memory to a new TriviaNode. Please remember to check that a new triviaNode is successfully created.</li>

 <li><strong>Step 5:</strong> Design and implement a function that asks a question to the player, input the player’s answer, and check if the player’s answer matches the actual answer. If so, award the player the dollar amount for that question. If the player enters the wrong answer your program should display the correct answer. o Input: a linked list of TriviaNode, the number of trivia to be asked in the list.  o Output: void or int  –  0 indicates success and 1 indicate failure.</li>

 <li><strong>Step 6:</strong> Write a test driver to perform unit testing for the function implemented in Step 5. Assume there are three trivia in your created list, you must cover at least the following cases: (see <strong> 1</strong> on page 3 for the sample user interface.) o Case 1: ask 0 question.

  <ul>

   <li>Case 2: ask 1 question (i.e., the first one) from the list.

    <ul>

     <li>Correct answer</li>

     <li>Wrong answer</li>

    </ul></li>

   <li>Case 3: ask 3 questions (i.e., all the questions) from the list.

    <ul>

     <li>Correct answers</li>

     <li>Wrong answers</li>

    </ul></li>

   <li>Case 4: ask 5 questions that exceed the number of available trivia in the linked list (i.e., the index of the trivia is larger than the array size).</li>

  </ul></li>

 <li><strong>Step 7:</strong> Write the main function that performs the following: (see Fig. 2 on page</li>

</ul>

4 for the sample user interface) o Create hard-code trivia quizzes (i.e., questions/answers/awards)  (Note: just call the function implemented in step 3). o Create more than 1 trivia quiz from a keyboard (Note: just call the function implemented in step 4).

o Write a for loop; in each iteration do the following:

<ul>

 <li>asks a question to the player,</li>

 <li>input the player’s answer,</li>

 <li>if the player’s answer matches the actual answer, then award the player the award points for that question</li>

 <li>else (i.e., the player enters the wrong answer) your program should display the correct answer. o When all questions have been asked display the total award points the player has won.</li>

 <li><strong>Step 8:</strong> Creating two versions using conditional compilation.</li>

 <li>Version 1: simply run the test driver implemented in Step 6.</li>

 <li>Version 2: a regular version run the main function implemented in Step 7. Note: this version does not include the test driver.</li>

</ul>

You must provide the following user interface for the <strong>debug version</strong>. The user input is depicted as <strong>Bold</strong>, but you do not need to display user input in bold. In this version, your program must run the test driver you build in Step 6.




<table width="0">

 <tbody>

  <tr>

   <td width="576">*** This is a debugging version ***Unit Test Case 1: Ask nomessage.  question. The program should give a warning<strong>Warning – The number of trivia to be asked must equal to or larger </strong> <strong>than 1. </strong><strong>  </strong>Unit Test Case 2.1: Ask 1 question in the linked list. The tester <sup> </sup>enters an incorrect answer.Question: How long was the shortest war on record? (Hint: how many  minutes)Answer: <strong>85</strong> Case 2.1 passed… Unit Test Case 2.2: Ask 1 question in the linked list. The tester  enters a correct answer.Question: What is the best-selling video game of all time? (Hint: Call of Duty or Wii Sports)?Answer: <strong>Wii Sports</strong> Case 2.2 passed… Unit Test Case 3: Ask all the questions of the last trivia in the linked list.Question: What is the best-selling video game of all time? (Hint: Call of Duty or Wii Sports)?Answer: <strong>Call of Duty </strong> show question here  Add your answer here … Unit Test Case 4: Ask five questions in the linked list.  <strong>Warning – There are only three trivia in the list. </strong> *** End of the Debugging Version ***</td>

  </tr>

 </tbody>

</table>

<strong>Fig. 1. Sample user interface for the debug version. </strong>

You must provide the following user interface for the <strong>production version</strong>. The user input is depicted as <strong>Bold</strong>, but you do not need to display user input in bold. Please replace “Li” with your name. In this version, your program must run the test driver you build in Step

<ol start="6">

 <li></li>

</ol>

<table width="0">

 <tbody>

  <tr>

   <td width="576"> *** Welcome to <strong>Li’s</strong> trivia quiz game ***Enter a question: enter your first question here.Enter an answer: enter your first answer here.Enter award points: enter your first award points here.<sup> </sup>Continue? (Yes/No): <strong>Yes</strong>Enter a question: enter your second question here.   Enter an answer: enter your second answer here.<sub> </sub>Enter award points: Continue? (Yes/No): enter your <strong>No</strong>       second award points here. Question: How long was the shortest war on record? (Hint: how many  minutes)Answer: <strong>38</strong>Your answer is correct. You receive 100 points.Your total points: 100<sub> </sub>Question: Italy or Bank of What was Bank of America’s original name? (Hint: Bank of Germany)?Answer: <strong>Bank of Germany</strong>Your answer is wrong. The correct answer is: Bank of ItalyYour Total points: 100Question: What is the best-selling video game of all time? (Hint:  Call of Duty or Wii Sports)?Answer: <strong>Wii Sports</strong>Your answer is correct. You receive 120 points.<sup> </sup>Your total points: 120 …Display more questions/answers and information here…… *** Thank you for playing the trivia quiz game. Goodbye! ***</td>

  </tr>

 </tbody>

</table>

<strong>Fig. 2. Sample user interface for the production version. </strong>




<strong><em><u>How to Create Two Versions?</u> </em></strong>

You can use the preprocessor directive #ifdef to create and maintain two versions (i.e., a debugging version and a product version) in your program. If you have the sequence




#ifdef UNIT_TESTING

add your unit testing code here

#else

add your code for the product version here

#endif




in your program, the code that is compiled depends on whether a preprocessor macro by that name is defined or not. For example, if there has been a “#define UNIT_TESTING” macro line), then “ add your unit testing code here ” is compiled and “ add your code for the product version here ” is ignored. If the macro is not defined, “ add your code for the product version here ” is compiled and “ add your unit testing code here ” is ignored.




These macros look a lot like if statements, but macros behave completely differently. More specifically, an if statement decides which statements of your program must be executed at run time; #ifdef controls which lines of code in your program are actually compiled.




<strong><em><u>Unit Testing:</u> </em></strong>

Unit testing is a way of determining if an individual function or class works. You need to isolate a single function or class and test only that function or class. For each function in this homework, you need to check <u>normal cases and boundary cases.</u>




Examples for tested values:

<ul>

 <li>string – empty string, medium length, very long</li>

 <li>Array – empty array, first element, last element</li>

 <li>Int – zero, mid-value, high-value</li>

</ul>




You must implement a unit test driver for each function implemented in your program. You may need to use assert() to develop your unit test drivers if tested results are predictable.




<strong><em><u>Integration Testing:</u> </em></strong>

Integration testing (a.k.a., Integration and Testing) is the phase in software testing in which individual software modules are combined and tested as a group. You may use the sample user interface illustrated in Fig. 2 on page 4 to perform an integration testing for your program.

<strong><em><u>Requirements:</u> </em></strong>

<ol>

 <li> Use comments to provide a heading at the top of your code containing your name, Auburn Userid, filename, and how to compile your code. Also describe any help or sources that you used (as per the syllabus).</li>

 <li> Your source code file should be named as “project4_AU UserID.cpp”</li>

 <li> Your program must use structures and a linked list. (see steps 1-2)</li>

 <li>Your program must use string rather than char array. (see steps 1-2)</li>

 <li> A function that creates 3 hard-coding trivia quizzes. (see step 3)</li>

 <li> A function that creates new quiz from a keyboard. (see step 4)</li>

 <li>A function that asks a question and checks a player’s answer. (see step 5)</li>

 <li>Write a test driver for function implemented in Step 5.</li>

 <li> Correctly implement the main function. (step 7).</li>

 <li> Creating two versions using conditional compilation.</li>

 <li> You must reduce the number of global variables and data 12. (5 points) Usability of your program (e.g., user interface)</li>

 <li> Readability of your source code.</li>

</ol>

Note: You will lose <strong>at least 40 points</strong> if there are compilation errors or warning messages when the TA compiles your source code. You will lose points if you: do not use the specific program file name, or do not have a comment on each function in your program you hand in.




<strong><em><u>Programming Environment:</u> </em></strong>

Write a short program in C++.  Compile and run it using AU server (no matter what kind of text editor you use, please make sure your code could run on AU server, the only test bed we accept is AU server).

<strong><em> </em></strong>

<strong><em><u>Deliverables:</u> </em></strong>