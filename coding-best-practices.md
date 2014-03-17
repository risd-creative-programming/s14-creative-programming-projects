#Week 5 - Mar 17: Workshop 2
#Creative Coding Best Practices

##Time management

![](http://i.imgur.com/aQZHy.gif)

* [Quora: Why are software development task estimations regularly off by a factor of 2-3?](http://www.quora.com/Engineering-Management/Why-are-software-development-task-estimations-regularly-off-by-a-factor-of-2-3)  
Read the top voted answer with 8.9k votes by Michael Wolfe
* [Bocoup Blog: Time Estimation, Software, and Dinner](http://weblog.bocoup.com/time-estimation-software-and-dinner/)

##Version control

* DIY -- copy the folder and rename with date.
* Github

##Code organization

* **Name well** -- Make sure variable names reflect what they describe on screen, class/object names reflect what they are, and function names reflect what they do.
* **Comment** -- Describe what's going on in English your parents can understand. Go line-by-line in your code if you have to. The more self-explanatory your variable/function names, the simpler your comments can be. It may seem obvious to you at the moment, but if you come back to your code hours, days, weeks, years later, you will thank yourself!
* **DRY** -- Don’t Repeat Yourself. Make variables for number values or functions for blocks of repeated code so you can make a change without having to update 5 different spots.
* **Modularize** -- Organize your code into functions so your code is easier to read and you can turn functionality on/off more easily. When your project starts to get larger, split your code into multiple files instead of having one really long file.
* **Format** -- Format your code early and often, line up if blocks, for loops, and functions. This will help you (and anyone you ask for help) to see and understand what’s going on. (Cmd/ctrl+t in Processing will do it automatically for you!)

##Common errors

* [https://www.iiitd.edu.in/~jalote/papers/CommonBugs.pdf](https://www.iiitd.edu.in/~jalote/papers/CommonBugs.pdf)
* **Compilation errors** -- Errors that stop your program from compiling. In Processing, openFrameworks, etc when you try to run the code will not compile and start. In JavaScript, the code will likely run until it hits the incorrect line in your code. Most compiler errors are caused by mistakes that you make when typing code. For example, you might misspell a keyword, leave out some necessary punctuation, or try to use an End If statement without first using an If statement.
* **Runtime errors** -- Errors that occur while your program runs. These typically occur when your program attempts an operation that is impossible to carry out. An example of this is division by zero, an infinite for loop. Technically, all JS errors are runtime errors.
* **Logic errors** -- Errors that prevent your program from doing what you intended it to do. Your code may compile and run without error, but the result of an operation may produce a result that you did not expect.

##Activity 1: Common errors

**Part 1**: As a group, create a list of common errors. (~10 mins)  
* null pointer [http://wiki.processing.org/w/Why_do_I_get_a_NullPointerException%3F](http://wiki.processing.org/w/Why_do_I_get_a_NullPointerException%3F)
* confusing = and ==
* undeclared function
* off by one error
* array out of bounds
* arithmetic errors
* 

**Part 2**: Each person picks one error. Create a diagram / illustration of the error. Could be more conceptual… should not be code example. Show diagram to class, explain what the error is, how to detect it, etc. (~20 mins)

##Debugging strategies

* **Error messages** -- Read the error messages. Don’t be worried if you don’t know what they mean, google can help you!
* **Comment out** -- Temporarily comment chunks of code in and out to track down the problem area.
* **Simplify** -- Get rid of all code except for the bare minimum required to demonstrate what's going wrong.
* **Print** -- Print out any and all values that might help you better understand what's going on. Label what you're printing using String concatenation.
* **Talk it out** -- Find a friend and talk through your problem. They don’t necessarily need to completely understand your code. Sometimes just walking step by step through a problem can make you see a detail or solution you were overlooking.
    * [Rubber duck debugging](debugging http://en.wikipedia.org/wiki/Rubber_duck_debugging)
* **Ask for help** -- Don’t waste hours or days stuck on a problem. If you have tried all the above yourself and looked around online, ask for help. Places to ask include forums, IRC, mailing lists, classmates.
* **Step by step** -- walk through this process. (Adapted from Clay Shirky’s [A Brief Introduction to Debugging](https://docs.google.com/document/d/1ZekLDsbLpySJgFvYYtpYmWMEQ3kiUNW6fOt7BNmTHX8/edit).)

###Prepare

+ Don’t panic. (Do take a deep breath.)  
+ Take a snapshot. Don’t go backwards! Keep track of everything you try.  
+ Write a message asking for help.  
  
###Observe

![text](http://i.imgur.com/WIrUykX.gif)

+ Is everything plugged in?
+ What just changed?
+ Read the code like a computer.
+ What do the error messages say? Read the error messages. Don’t be worried if you don’t know what they mean, google can help you!
+ LMGTFY
+ Print -- Print out any and all values that might help you better understand what's going on. Label what you're printing using String concatenation.

###Change
+ Can you work from one end to the other?
+ Write your own error reporting
+ Process of Elimination 
     + Comment out -- Temporarily comment chunks of code in and out to track down the problem area.
     + Simplify -- Get rid of all code except for the bare minimum required to demonstrate what's going wrong.
+ Sanity check: are you looking at the same thing you are changing?

###Defend 
+ Premature Optimization Is The Root of All Evil  
+ Only do one thing at a time  
+ Save working versions  

###Be social
+ __Ask for help__ -- Don’t waste hours or days stuck on a problem. If you have tried all the above yourself and looked around online, ask for help. Places to ask include forums, IRC, mailing lists, classmates. See below for tips for asking for help.
+ __Talk it out__ -- Find a friend and talk through your problem. They don’t necessarily need to completely understand your code. Sometimes just walking step by step through a problem can make you see a detail or solution you were overlooking.
    + [Rubber duck debugging](http://en.wikipedia.org/wiki/Rubber_duck_debugging)


##Asking for help

![](https://31.media.tumblr.com/d586c5f898287597dc01facc77d7a8a4/tumblr_inline_mzjzs15gYy1qj3ir1.gif)

* Try something first. You should be asking for help, not a solution. 
          [whathaveyoutried.com](http://www.whathaveyoutried.com)
* Narrow down the problem, create a miniature version that isolates what’s going wrong.
* Provide enough detail. Provide a specific, concise code example and error message if you have one.
* Don’t be lazy. Check for typos, silly mistakes. See step by step above.
* Be patient and not demanding.

* More resources
    * [How to ask for programming help](http://codingkilledthecat.wordpress.com/2012/06/26/how-to-ask-for-programming-help/)
    * [How to ask questions the smart way](http://www.catb.org/esr/faqs/smart-questions.html)
    * [Getting help on IRC](https://workaround.org/getting-help-on-irc)

##Activity 2: Debug Competition

**Part 1**: Break into teams of 2 (make sure each group has one person that knows Processing or code well). Create a Processing sketch, and take a screenshot of the output. Then change only one line / insert one bug of the sketch code to “break” it. Broken could mean it won’t run or it looks wrong, compared to the screenshot you took. (~20 minutes)

**Part 2**: Each team of 2 will be given a different team’s sketch and desired output screenshot, and try to debug/unbreak it as fast as possible (get it to run and match the output of the screenshot). Repeat once more with another team’s sketch.  (~30 mins)

**Part 3**: We add up the times to debug each sketch, “winning team” is the team whose sketch took the longest / was the hardest to debug. Debrief and discuss. (~20 mins)
* What types of errors did we see?
* Which were hardest to find?
* Which were easiest?
* What strategies did you use?
* How did we think about writing a sketch to be hard to debug / hide an error?
* What realizations did you have while creating or debugging?

##More resources
* Excellent article on [how to approach problem-solving](http://mattgemmell.com/2008/12/08/what-have-you-tried/)
* Clay Shirky's guide to the [Basics of Debugging](https://docs.google.com/document/d/1ZekLDsbLpySJgFvYYtpYmWMEQ3kiUNW6fOt7BNmTHX8/edit)
* [whathaveyoutried.com](http://www.whathaveyoutried.com)
