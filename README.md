Download Link: https://assignmentchef.com/product/solved-prog1360-assignment-3-blinking-lights
<br>
<h3>Demonstration – Building on Labs</h3>

This assignment builds on the labs and assignments so far.

The Demonstration section of this document outlines the items you are required to show.

Tasks

You will implement a simple game that uses the lights and button on the board.

Given the command below (where xx is your initials)

xxGame delay pattern target

your board will repeatedly blink the lights in the pattern you specify, until you push the button. If when you push the button the target light is on, the user “wins” and all the lights blink twice at the same time. If the user loses, only the target light is lit up.

Example:

jsGame 500 43567011 5

This would run the game with a delay of 500ms between lights (you will have to scale the delay) and cycle the lights in a pattern of 4, 3, 5, 6, 7, 0, 1, 1. If the user manages to push the button when the 5 light is lit up, they will win.

<h3>Requirements</h3>

<ul>

 <li>No logic is to be implemented in your C hook code UNLESS it is related to removing the busy delay.</li>

 <li>You may use library functions from the stm32 code to detect button state and parse input.</li>

 <li>It is very important that you structure your code cleanly for this assignment.</li>

 <li>You must name all functions and adapt any menu help instructions appropriately.</li>

 <li>You will have to scale the delay to approximate milliseconds.</li>

 <li>You will have to parse the input pattern and store it in a way that you can cycle through it repeatedly.</li>

</ul>

<h2>Demonstration</h2>

Please note that you must be prepared before offering to demonstrate your code. You must demonstrate the code that you have submitted to the eConestoga dropbox.

For this assignment, you will demonstrate the following items. You may use a lab PC or your own. If needed, you may use a classmate’s VM, but you MUST run your own code and only your own code. You must demonstrate in your regularly scheduled lab period. If you demonstrate modified code, you will receive a late penalty according to how long it has been since the dropbox deadline.

<ol>

 <li>Your xx_hook.c and xx_asm.s code as taken directly from the drop box compiles.</li>

 <li>Your code deploys with make program.</li>

 <li>Your code runs with no parameters provided (sensible defaults).</li>

 <li>Your code runs as specified.</li>

 <li>You can demonstrate both cases – that it is possible to both win and lose.</li>

</ol>

<h2>Code</h2>

The code you submit will be evaluated on the following criteria.

<h3>Functionality</h3>

Your program behaves as specified.

<h3>Proper use of Registers, the stack, and link register</h3>

Only necessary items (no more, no less) are pushed onto the stack. Your function calls use the link register appropriately.

<h3>Code Readability and Structure</h3>

Your code is properly indented, does not wrap or have long lines, and can be logically understood.

You use subroutines and memory appropriately.

<h3>Code comments</h3>

As this is assembly language, you must extensively comment any code that is unclear (i.e. nearly every line).








