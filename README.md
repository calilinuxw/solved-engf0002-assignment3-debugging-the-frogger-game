Download Link: https://assignmentchef.com/product/solved-engf0002-assignment3-debugging-the-frogger-game
<br>
In the mhandley/ENGF0002-2019 github repository, in the

Assignments/assignment3 directory, there are a number of python and PNG files that together comprise an implementation of the 1980s video game <em>Frogger</em>. The game is written in an object oriented style, and roughly conforms to a Model/View/Controller design pattern, as discussed in class. Run the game by typing:

python3 frogger.py

or the equivalent on your system. On the lab Linux machines, a new version of python 3 is in /opt/Python/Python-3.7/bin/python. The game does work using the departmental Linux machines using CSRW, though it does jitter a bit.

The objective of the game is to cross the road, avoiding the cars, cross the river by jumping on the logs or turtles, and make it to one of the five frog homes at the top of the screen. You start out with seven lives and a certain amount of time. You must get frogs to all five homes before the time runs out, or it’s Game Over. If you succeed in filling all five homes, you get to move on to the next level, and the game gets a little harder.

The game requires python 3 and a recent enough version of tkinter that has PNG support.

The problem is that the game has at least five bugs that make it unplayable. Your task:

<ol>

 <li>Play the game.</li>

 <li>Find a bug.</li>

 <li>Write a brief bug report describing the bug.</li>

 <li>Identify the cause of the bug. Write a brief summary of the cause.</li>

 <li>Fix the bug.</li>

 <li>Repeat from 1.</li>

</ol>

<h2>Bug Reports</h2>

A bug report should be brief and to the point. It should include:

<ul>

 <li>One sentence summary of the bug.</li>

 <li>Description of what happens.</li>

 <li>Description of what you think should happen.</li>

 <li>Instructions for how to reproduce the bug.</li>

</ul>

<h2>Understanding the bug</h2>

Once you’ve written the bug report, look at the code.

Identify what the code is doing when the bug is triggered. Sometimes the cause may be obvious from reading the code. Often the cause is not obvious, and even the flow of the code may not be obvious. Then you will need to instrument the code to figure out what it is doing. In this case, I just want you to instrument the code using print() – there’s no need to use a debugger. Generally, you want to instrument the code without changing its behaviour until you gather enough information to understand what the code is actually doing (and hence why it differs from what it should be doing).

You may however want to temporarily change the code to make it easier to reproduce a bug, and then revert those changes after you’ve fixed the bug. A common debugging technique is to reduce the code complexity by removing code to reduce it to the simplest case that still exhibits the buggy behaviour. This is a valuable technique when a bug is hard to reproduce.

In general, you’re hunting for evidence until you’ve found out what the program is actually doing. Only when you understand what the program is doing should you think about how to fix it.

<h2>Fixing the bugs</h2>

These bugs are very simple. Some are one line fixes, none requires more than about three lines of extra code to fix. One will require you read the code very carefully.

<h2>Assessment</h2>

This assignment is not assessed. The purpose of the assignment is to give you practice reading, understanding, and debugging a non-trivial piece of code. You many work with your friends on this assignment if you wish. You must hand in a reasonable attempt via Moodle to receive a binary mark, as we want to see how you are progressing. Hand in a zipfile containing the text of your bug reports, your brief explanations of the causes of the bugs, and the python source code of your fixed version of the game.

<h2>Optional Extra</h2>

A few members of the class are more experienced programmers. If you find fixing the bugs easy, once you’ve fixed them, consider extending the game. For example, in the original 1980s game, the turtles submerge every so often, and there are crocodiles and other hazards. Also the way the game gets harder with each level is somewhat better.

There will be a separate submission area on Moodle for game extensions. You won’t get any extra marks, but if we like your code enough to use next year, we’ll figure out some reward.