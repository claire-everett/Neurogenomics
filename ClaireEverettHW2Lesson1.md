> installed.packages(swirl)
Error in installed.packages(swirl) : object 'swirl' not found
> installed.packages'swirl')
Error: unexpected string constant in "installed.packages'swirl'"
> installed.packages('swirl')
Package LibPath Version Priority Depends Imports LinkingTo Suggests Enhances License License_is_FOSS
License_restricts_use OS_type Archs MD5sum NeedsCompilation Built
> library(swirl)
Error in library(swirl) : there is no package called ‘swirl’
> install.packages("swirl")
also installing the dependencies ‘praise’, ‘bitops’, ‘testthat’, ‘RCurl’

trying URL 'https://cran.rstudio.com/bin/macosx/el-capitan/contrib/3.6/praise_1.0.0.tgz'
Content type 'application/x-gzip' length 16379 bytes (15 KB)
==================================================
  downloaded 15 KB

trying URL 'https://cran.rstudio.com/bin/macosx/el-capitan/contrib/3.6/bitops_1.0-6.tgz'
Content type 'application/x-gzip' length 25079 bytes (24 KB)
==================================================
  downloaded 24 KB

trying URL 'https://cran.rstudio.com/bin/macosx/el-capitan/contrib/3.6/testthat_2.2.1.tgz'
Content type 'application/x-gzip' length 2324119 bytes (2.2 MB)
==================================================
  downloaded 2.2 MB

trying URL 'https://cran.rstudio.com/bin/macosx/el-capitan/contrib/3.6/RCurl_1.95-4.12.tgz'
Content type 'application/x-gzip' length 995934 bytes (972 KB)
==================================================
  downloaded 972 KB

trying URL 'https://cran.rstudio.com/bin/macosx/el-capitan/contrib/3.6/swirl_2.4.4.tgz'
Content type 'application/x-gzip' length 346278 bytes (338 KB)
==================================================
  downloaded 338 KB


The downloaded binary packages are in
/var/folders/2g/m234ml7x7c904pcbd0sxz_cr0000gp/T//RtmpyXWo0w/downloaded_packages
> library('swirl')

| Hi! Type swirl() when you are ready to begin.

> swirl()

| Welcome to swirl! Please sign in. If you've been here before, use the same name as you did then. If you are new,
| call yourself something unique.

What shall I call you? Claire

| Thanks, Claire. Let's cover a couple of quick housekeeping items before we begin our first lesson. First of all,
| you should know that when you see '...', that means you should press Enter when you are done reading and ready
| to continue.

...  <-- That's your cue to press Enter to continue

| Also, when you see 'ANSWER:', the R prompt (>), or when you are asked to select from a list, that means it's
| your turn to enter a response, then press Enter to continue.

Select 1, 2, or 3 and press Enter 

1: Continue.
2: Proceed.
3: Let's get going!

Selection: 1

| You can exit swirl and return to the R prompt (>) at any time by pressing the Esc key. If you are already at the
| prompt, type bye() to exit and save your progress. When you exit properly, you'll see a short message letting
| you know you've done so.

| When you are at the R prompt (>):
| -- Typing skip() allows you to skip the current question.
| -- Typing play() lets you experiment with R on your own; swirl will ignore what you do...
| -- UNTIL you type nxt() which will regain swirl's attention.
| -- Typing bye() causes swirl to exit. Your progress will be saved.
| -- Typing main() returns you to swirl's main menu.
| -- Typing info() displays these options again.

| Let's get started!
  
  ...skip()

| To begin, you must install a course. I can install a course for you from the internet, or I can send you to a
| web page (https://github.com/swirldev/swirl_courses) which will provide course options and directions for
| installing courses yourself. (If you are not connected to the internet, type 0 to exit.)

1: R Programming: The basics of programming in R
2: Regression Models: The basics of regression modeling in R
3: Statistical Inference: The basics of statistical inference in R
4: Exploratory Data Analysis: The basics of exploring data in R
5: Don't install anything for me. I'll do it myself.

Selection: 1
|=========================================================================================================| 100%

| Course installed successfully!
  
  
  | Please choose a course, or type 0 to exit swirl.

1: R Programming
2: Take me to the swirl course repository!
  
  Selection: 1

| Please choose a lesson, or type 0 to return to course menu.

1: Basic Building Blocks      2: Workspace and Files        3: Sequences of Numbers    
4: Vectors                    5: Missing Values             6: Subsetting Vectors      
7: Matrices and Data Frames   8: Logic                      9: Functions               
10: lapply and sapply         11: vapply and tapply         12: Looking at Data         
13: Simulation                14: Dates and Times           15: Base Graphics           


Selection: 1

|                                                                                                         |   0%

| In this lesson, we will explore some basic building blocks of the R programming language.

...

|===                                                                                                      |   3%
| If at any point you'd like more information on a particular topic related to R, you can type help.start() at the
| prompt, which will open a menu of resources (either within RStudio or your default web browser, depending on
| your setup). Alternatively, a simple web search often yields the answer you're looking for.

...

|======                                                                                                   |   5%
| In its simplest form, R can be used as an interactive calculator. Type 5 + 7 and press Enter.

> 5+7
[1] 12

| That's correct!

  |========                                                                                                 |   8%
| R simply prints the result of 12 by default. However, R is a programming language and often the reason we use a
| programming language as opposed to a calculator is to automate some process or avoid unnecessary repetition.

...

  |===========                                                                                              |  11%
| In this case, we may want to use our result from above in a second calculation. Instead of retyping 5 + 7 every
| time we need it, we can just create a new variable that stores the result.

...

  |==============                                                                                           |  13%
| The way you assign a value to a variable in R is by using the assignment operator, which is just a 'less than'
| symbol followed by a 'minus' sign. It looks like this: <-

...x <- 5 + 7

  |=================                                                                                        |  16%
| Think of the assignment operator as an arrow. You are assigning the value on the right side of the arrow to the
| variable name on the left side of the arrow.

...

  |===================                                                                                      |  18%
| To assign the result of 5 + 7 to a new variable called x, you type x <- 5 + 7. This can be read as 'x gets 5
| plus 7'. Give it a try now.

> x <- 5 + 7

| Excellent job!

  |======================                                                                                   |  21%
| You'll notice that R did not print the result of 12 this time. When you use the assignment operator, R assumes
| that you don't want to see the result immediately, but rather that you intend to use the result for something
| else later on.

...

  |=========================                                                                                |  24%
| To view the contents of the variable x, just type x and press Enter. Try it now.

> x
[1] 12

| That's correct!
  
  |============================                                                                             |  26%
| Now, store the result of x - 3 in a new variable called y.

> y <- x - 3

| Nice work!
  
  |==============================                                                                           |  29%
| What is the value of y? Type y to find out.

> y
[1] 9

| That's a job well done!

  |=================================                                                                        |  32%
| Now, let's create a small collection of numbers called a vector. Any object that contains data is called a data
| structure and numeric vectors are the simplest type of data structure in R. In fact, even a single number is
| considered a vector of length one.

...

|====================================                                                                     |  34%
| The easiest way to create a vector is with the c() function, which stands for 'concatenate' or 'combine'. To
| create a vector containing the numbers 1.1, 9, and 3.14, type c(1.1, 9, 3.14). Try it now and store the result
| in a variable called z.

> 
  > z <- c(1.1, 9, 3,14)

| You're close...I can feel it! Try it again. Or, type info() for more options.

| Inputting z <- c(1.1, 9, 3.14) will assign the vector (1.1, 9, 3.14) to a new variable called z. Including
| single spaces after the commas in the vector is not required, but helps make your code less cluttered and more
| readable.

> z <- c(1.1, 9, 3.14)

| You're the best!
  
  |=======================================                                                                  |  37%
| Anytime you have questions about a particular function, you can access R's built-in help files via the `?`
| command. For example, if you want more information on the c() function, type ?c without the parentheses that
| normally follow a function name. Give it a try.

> ?c

| You got it!

  |=========================================                                                                |  39%
| Type z to view its contents. Notice that there are no commas separating the values in the output.

> z
[1] 1.10 9.00 3.14

| Nice work!

  |============================================                                                             |  42%
| You can combine vectors to make a new vector. Create a new vector that contains z, 555, then z again in that
| order. Don't assign this vector to a new variable, so that we can just see the result immediately.

> c(z, 55, z)
[1]  1.10  9.00  3.14 55.00  1.10  9.00  3.14

| That's not exactly what I'm looking for. Try again. Or, type info() for more options.

| Type c(z, 555, z). Don't create a new variable. We just want to view the result.

> c(z, 555, z)
[1]   1.10   9.00   3.14 555.00   1.10   9.00   3.14

| Excellent work!

  |===============================================                                                          |  45%
| Numeric vectors can be used in arithmetic expressions. Type the following to see what happens: z * 2 + 100.

> z * 2 + 100
[1] 102.20 118.00 106.28

| That's correct!
  
  |==================================================                                                       |  47%
| First, R multiplied each of the three elements in z by 2. Then it added 100 to each element to get the result
| you see above.

...

|====================================================                                                     |  50%
| Other common arithmetic operators are `+`, `-`, `/`, and `^` (where x^2 means 'x squared'). To take the square
| root, use the sqrt() function and to take the absolute value, use the abs() function.

...

|=======================================================                                                  |  53%
| Take the square root of z - 1 and assign it to a new variable called my_sqrt.

> my+sqrt <- sqrt(z-1)
Error in my + sqrt <- sqrt(z - 1) : object 'my' not found
> my_sqrt <- sqrt(z-1)

| Nice work!
  
  |==========================================================                                               |  55%
| Before we view the contents of the my_sqrt variable, what do you think it contains?
  
  1: a single number (i.e a vector of length 1)
2: a vector of length 0 (i.e. an empty vector)
3: a vector of length 3

Selection: 3

| You're the best!

  |=============================================================                                            |  58%
| Print the contents of my_sqrt.

> my_sqrt
[1] 0.3162278 2.8284271 1.4628739

| That's a job well done!
  
  |================================================================                                         |  61%
| As you may have guessed, R first subtracted 1 from each element of z, then took the square root of each element.
| This leaves you with a vector of the same length as the original vector z.

...

|==================================================================                                       |  63%
| Now, create a new variable called my_div that gets the value of z divided by my_sqrt.

> my_div <- z/my_squrt
Error: object 'my_squrt' not found
> my_div <- z/my_sqrt

| You are really on a roll!
  
  |=====================================================================                                    |  66%
| Which statement do you think is true?
  
  1: The first element of my_div is equal to the first element of z divided by the first element of my_sqrt, and so on...
2: my_div is undefined
3: my_div is a single number (i.e a vector of length 1)

Selection: 1

| Keep working like that and you'll get there!

  |========================================================================                                 |  68%
| Go ahead and print the contents of my_div.

> my_div
[1] 3.478505 3.181981 2.146460

| That's a job well done!
  
  |===========================================================================                              |  71%
| When given two vectors of the same length, R simply performs the specified arithmetic operation (`+`, `-`, `*`,
                                                                                                   | etc.) element-by-element. If the vectors are of different lengths, R 'recycles' the shorter vector until it is
| the same length as the longer vector.

...

|=============================================================================                            |  74%
| When we did z * 2 + 100 in our earlier example, z was a vector of length 3, but technically 2 and 100 are each
| vectors of length 1.

...

|================================================================================                         |  76%
| Behind the scenes, R is 'recycling' the 2 to make a vector of 2s and the 100 to make a vector of 100s. In other
| words, when you ask R to compute z * 2 + 100, what it really computes is this: z * c(2, 2, 2) + c(100, 100,
                                                                                                    | 100).

...

|===================================================================================                      |  79%
| To see another example of how this vector 'recycling' works, try adding c(1, 2, 3, 4) and c(0, 10). Don't worry
| about saving the result in a new variable.

> c(1, 2, 3, 4) + c(0, 10)
[1]  1 12  3 14

| Nice work!

  |======================================================================================                   |  82%
| If the length of the shorter vector does not divide evenly into the length of the longer vector, R will still
| apply the 'recycling' method, but will throw a warning to let you know something fishy might be going on.

...

  |========================================================================================                 |  84%
| Try c(1, 2, 3, 4) + c(0, 10, 100) for an example.

> c(1, 2, 3, 4) _ c(0, 10, 100)
Error: unexpected input in "c(1, 2, 3, 4) _"
> 
> c(1, 2, 3, 4) + c(0, 10, 100)
[1]   1  12 103   4
Warning message:
In c(1, 2, 3, 4) + c(0, 10, 100) :
  longer object length is not a multiple of shorter object length

| Perseverance, that's the answer.

|===========================================================================================              |  87%
| Before concluding this lesson, I'd like to show you a couple of time-saving tricks.

...

  |==============================================================================================           |  89%
| Earlier in the lesson, you computed z * 2 + 100. Let's pretend that you made a mistake and that you meant to add
| 1000 instead of 100. You could either re-type the expression, or...

...

|=================================================================================================        |  92%
| In many programming environments, the up arrow will cycle through previous commands. Try hitting the up arrow on
| your keyboard until you get to this command (z * 2 + 100), then change 100 to 1000 and hit Enter. If the up
| arrow doesn't work for you, just type the corrected command.

> z * 2 + 1000
[1] 1002.20 1018.00 1006.28

| All that practice is paying off!

  |===================================================================================================      |  95%
| Finally, let's pretend you'd like to view the contents of a variable that you created earlier, but you can't
| seem to remember if you named it my_div or myDiv. You could try both and see what works, or...

...

|======================================================================================================   |  97%
| You can type the first two letters of the variable name, then hit the Tab key (possibly more than once). Most
| programming environments will provide a list of variables that you've created that begin with 'my'. This is
| called auto-completion and can be quite handy when you have many variables in your workspace. Give it a try. (If
| auto-completion doesn't work for you, just type my_div and press Enter.)

> my_div
[1] 3.478505 3.181981 2.146460

| All that hard work is paying off!
  
  |=========================================================================================================| 100%
  | Would you like to receive credit for completing this course on Coursera.org?
    
    1: Yes
  2: No
  
  Please choose a course, or type 0 to exit swirl.
  
  1: R Programming
  2: Take me to the swirl course repository!
    
    Selection: 1
  
  | Please choose a lesson, or type 0 to return to course menu.
  
  1: Basic Building Blocks      2: Workspace and Files        3: Sequences of Numbers    
  4: Vectors                    5: Missing Values             6: Subsetting Vectors      
  7: Matrices and Data Frames   8: Logic                      9: Functions               
  10: lapply and sapply         11: vapply and tapply         12: Looking at Data         
  13: Simulation                14: Dates and Times           15: Base Graphics           
  
  
  Selection: 2
  
  |                                                                                                         |   0%
  
  | In this lesson, you'll learn how to examine your local workspace in R and begin to explore the relationship
| between your workspace and the file system of your machine.

...

  |===                                                                                                      |   3%
| Because different operating systems have different conventions with regards to things like file paths, the
| outputs of these commands may vary across machines.

...

  |=====                                                                                                    |   5%
| However it's important to note that R provides a common API (a common set of commands) for interacting with
  | files, that way your code will work across different kinds of computers.
  
  ...
  
  |========                                                                                                 |   8%
  | Let's jump right in so you can get a feel for how these special functions work!

...

  |===========                                                                                              |  10%
| Determine which directory your R session is using as its current working directory using getwd().

> getwd()
[1] "/Users/Claire/Desktop/Neurogenomics"

| You're the best!
    
    |=============                                                                                            |  13%
  | List all the objects in your local workspace using ls().
  
  > ls()
  [1] "my_div"  "my_sqrt" "x"       "y"       "z"      
  
  | That's a job well done!

  |================                                                                                         |  15%
| Some R commands are the same as their equivalents commands on Linux or on a Mac. Both Linux and Mac operating
| systems are based on an operating system called Unix. It's always a good idea to learn more about Unix!
    
    ...
  
  |===================                                                                                      |  18%
  | Assign 9 to x using x <- 9.
  
  > x <- 9
  
  | You are quite good my friend!
    
    |======================                                                                                   |  21%
  | Now take a look at objects that are in your workspace using ls().
  
  > ls()
  [1] "my_div"  "my_sqrt" "x"       "y"       "z"      
  
  | All that hard work is paying off!
    
    |========================                                                                                 |  23%
  | List all the files in your working directory using list.files() or dir().
  
  > list.files()
  [1] "Neurogenomics.Rproj" "README.md"          
  
  | Your dedication is inspiring!
    
    |===========================                                                                              |  26%
  | As we go through this lesson, you should be examining the help page for each new function. Check out the help
  | page for list.files with the command ?list.files.
  
  > ?list.files
  
  | Your dedication is inspiring!
    
    |==============================                                                                           |  28%
  | One of the most helpful parts of any R help file is the See Also section. Read that section for list.files. Some
  | of these functions may be used in later portions of this lesson.
  
  ...
  
  |================================                                                                         |  31%
  | Using the args() function on a function name is also a handy way to see what arguments a function can take.
  
  ...
  
  |===================================                                                                      |  33%
  | Use the args() function to determine the arguments to list.files().
  
  > args(list.files)
  function (path = ".", pattern = NULL, all.files = FALSE, full.names = FALSE, 
            recursive = FALSE, ignore.case = FALSE, include.dirs = FALSE, 
            no.. = FALSE) 
    NULL
  
  | You are really on a roll!
    
    |======================================                                                                   |  36%
  | Assign the value of the current working directory to a variable called "old.dir".
  
  > old.dir <- getwd()
  
  | You are quite good my friend!
    
    |========================================                                                                 |  38%
  | We will use old.dir at the end of this lesson to move back to the place that we started. A lot of query
  | functions like getwd() have the useful property that they return the answer to the question as a result of the
  | function.
  
  ...
  
  |===========================================                                                              |  41%
  | Use dir.create() to create a directory in the current working directory called "testdir".
  
  > dir.create()
  Error in dir.create() : argument "path" is missing, with no default
  > testdir = dir.create()
  Error in dir.create() : argument "path" is missing, with no default
  > dir.create()
  Error in dir.create() : argument "path" is missing, with no default
  > dir.create(testdir)
  Error in dir.create(testdir) : object 'testdir' not found
  > dir.create("testdir")
  
  | Excellent work!
    
    |==============================================                                                           |  44%
  | We will do all our work in this new directory and then delete it after we are done. This is the R analog to
  | "Take only pictures, leave only footprints."
  
  ...
  
  |================================================                                                         |  46%
  | Set your working directory to "testdir" with the setwd() command.
  
  > setwd("testdir")
  
  | That's a job well done!

  |===================================================                                                      |  49%
| In general, you will want your working directory to be someplace sensible, perhaps created for the specific
| project that you are working on. In fact, organizing your work in R packages using RStudio is an excellent
| option. Check out RStudio at http://www.rstudio.com/

...

  |======================================================                                                   |  51%
| Create a file in your working directory called "mytest.R" using the file.create() function.

> file.create("mytest.R")
[1] TRUE

| All that hard work is paying off!

  |=========================================================                                                |  54%
| This should be the only file in this newly created directory. Let's check this by listing all the files in the
  | current directory.
  
  > list.files()
  [1] "mytest.R"
  
  | You're the best!

  |===========================================================                                              |  56%
| Check to see if "mytest.R" exists in the working directory using the file.exists() function.

> file.exists("mytest.R")
[1] TRUE

| You are amazing!

  |==============================================================                                           |  59%
| These sorts of functions are excessive for interactive use. But, if you are running a program that loops through
| a series of files and does some processing on each one, you will want to check to see that each exists before
| you try to process it.

...

  |=================================================================                                        |  62%
| Access information about the file "mytest.R" by using file.info().

> file.infor("mytest.R")
Error in file.infor("mytest.R") : could not find function "file.infor"
> file.info("mytest.R")
         size isdir mode               mtime               ctime               atime uid gid  uname grname
mytest.R    0 FALSE  644 2019-09-20 12:32:54 2019-09-20 12:32:54 2019-09-20 12:32:56 502  20 Claire  staff

| You nailed it! Good job!

  |===================================================================                                      |  64%
| You can use the $ operator --- e.g., file.info("mytest.R")$mode --- to grab specific items.

...

  |======================================================================                                   |  67%
| Change the name of the file "mytest.R" to "mytest2.R" by using file.rename().

> file.rename("mytest2.R")
Error in file.rename("mytest2.R") : 
  argument "to" is missing, with no default
> file.rename("mytest.3", "mytest2.R")
[1] FALSE
Warning message:
In file.rename("mytest.3", "mytest2.R") :
  cannot rename file 'mytest.3' to 'mytest2.R', reason 'No such file or directory'

| Keep trying! Or, type info() for more options.

| file.rename("mytest.R", "mytest2.R") is the answer. Googling using key words from the question, along with the
| letter R, will often give you a good hint.

> file.rename("mytest.R", "mytest2.R")
[1] TRUE

| Excellent work!

  |=========================================================================                                |  69%
| Your operating system will provide simpler tools for these sorts of tasks, but having the ability to manipulate
| files programatically is useful. You might now try to delete mytest.R using file.remove('mytest.R'), but that
| won't work since mytest.R no longer exists. You have already renamed it.
  
  ...
  
  |===========================================================================                              |  72%
  | Make a copy of "mytest2.R" called "mytest3.R" using file.copy().
  
  > file.copy(mytest2.R, mytest3.R)
  Error in file.copy(mytest2.R, mytest3.R) : object 'mytest2.R' not found
  > list.files()
  [1] "mytest2.R"
  
  | You're close...I can feel it! Try it again. Or, type info() for more options.

| file.copy("mytest2.R", "mytest3.R") works.

> file.copy("mytest2.R", "mytest3.R" )
[1] TRUE

| That's the answer I was looking for.
  
  |==============================================================================                           |  74%
  | You now have two files in the current directory. That may not seem very interesting. But what if you were
  | working with dozens, or millions, of individual files? In that case, being able to programatically act on many
  | files would be absolutely necessary. Don't forget that you can, temporarily, leave the lesson by typing play()
| and then return by typing nxt().

...

  |=================================================================================                        |  77%
| Provide the relative path to the file "mytest3.R" by using file.path().

> file.path("mytest3.R")
[1] "mytest3.R"

| All that hard work is paying off!

  |===================================================================================                      |  79%
| You can use file.path to construct file and directory paths that are independent of the operating system your R
| code is running on. Pass 'folder1' and 'folder2' as arguments to file.path to make a platform-independent
| pathname.

> file.path('folder1', 'folder2')
[1] "folder1/folder2"

| You got it right!

  |======================================================================================                   |  82%
| Take a look at the documentation for dir.create by entering ?dir.create . Notice the 'recursive' argument. In
| order to create nested directories, 'recursive' must be set to TRUE.

> ?dir.create

| Keep working like that and you'll get there!
    
    |=========================================================================================                |  85%
  | Create a directory in the current working directory called "testdir2" and a subdirectory for it called
  | "testdir3", all in one command by using dir.create() and file.path().
  
  > file.path(dir.create("testdir2"), dir.create("testdir3"))
  [1] "TRUE/TRUE"
  
  | That's not the answer I was looking for, but try again. Or, type info() for more options.

| dir.create(file.path('testdir2', 'testdir3'), recursive = TRUE) will do the trick. If you forgot the recursive
| argument, the command may have appeared to work, but it didn't create the nested directory.
  
  > dir.create(file.path("testdir2","testdir3"), recursive = TRUE)
  
  | You got it!
    
    |============================================================================================             |  87%
  | Go back to your original working directory using setwd(). (Recall that we created the variable old.dir with the
                                                               | full path for the orginal working directory at the start of these questions.)
  
  > setwd(old.dir)
  
  | You got it!
    
    |==============================================================================================           |  90%
  | It is often helpful to save the settings that you had before you began an analysis and then go back to them at
  | the end. This trick is often used within functions; you save, say, the par() settings that you started with,
  | mess around a bunch, and then set them back to the original values at the end. This isn't the same as what we
| have done here, but it seems similar enough to mention.

...

  |=================================================================================================        |  92%
| After you finish this lesson delete the 'testdir' directory that you just left (and everything in it)

...

  |====================================================================================================     |  95%
| Take nothing but results. Leave nothing but assumptions. That sounds like 'Take nothing but pictures. Leave
  | nothing but footprints.' But it makes no sense! Surely our readers can come up with a better motto . . .

...

  |======================================================================================================   |  97%
| In this lesson, you learned how to examine your R workspace and work with the file system of your machine from
| within R. Thanks for playing!

 1: Basic Building Blocks      2: Workspace and Files        3: Sequences of Numbers    
 4: Vectors                    5: Missing Values             6: Subsetting Vectors      
 7: Matrices and Data Frames   8: Logic                      9: Functions               
10: lapply and sapply         11: vapply and tapply         12: Looking at Data         
13: Simulation                14: Dates and Times           15: Base Graphics           


Selection: 3

  |                                                                                                         |   0%

| In this lesson, you'll learn how to create sequences of numbers in R.
  
  ...
  
  |=====                                                                                                    |   4%
  | The simplest way to create a sequence of numbers in R is by using the `:` operator. Type 1:20 to see how it
  | works.
  
  > 1:20
  [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20
  
  | You are amazing!
    
    |=========                                                                                                |   9%
  | That gave us every integer between (and including) 1 and 20. We could also use it to create a sequence of real
  | numbers. For example, try pi:10.
  
  > pi:10
  [1] 3.141593 4.141593 5.141593 6.141593 7.141593 8.141593 9.141593
  
  | Nice work!
    
    |==============                                                                                           |  13%
  | The result is a vector of real numbers starting with pi (3.142...) and increasing in increments of 1. The upper
  | limit of 10 is never reached, since the next number in our sequence would be greater than 10.
  
  ...
  
  |==================                                                                                       |  17%
  | What happens if we do 15:1? Give it a try to find out.
  
  > 15:1
  [1] 15 14 13 12 11 10  9  8  7  6  5  4  3  2  1
  
  | Perseverance, that's the answer.

  |=======================                                                                                  |  22%
| It counted backwards in increments of 1! It's unlikely we'd want this behavior, but nonetheless it's good to
  | know how it could happen.
  
  ...
  
  |===========================                                                                              |  26%
  | Remember that if you have questions about a particular R function, you can access its documentation with a
  | question mark followed by the function name: ?function_name_here. However, in the case of an operator like the
  | colon used above, you must enclose the symbol in backticks like this: ?`:`. (NOTE: The backtick (`) key is
                                                                                 | generally located in the top left corner of a keyboard, above the Tab key. If you don't have a backtick key, you
| can use regular quotes.)

...

  |================================                                                                         |  30%
| Pull up the documentation for `:` now.

> help(':')

| You almost had it, but not quite. Try again. Or, type info() for more options.

| In order to view the documentation for a symbol like the colon operator, you have to use backticks (or quotes).
| This is so R knows you are not attempting to use the symbol in the command. Here's what it looks like: ?`:`.
                                                                                 | Don't forget the question mark out front.

> ':'
[1] ":"

| Keep trying! Or, type info() for more options.

| In order to view the documentation for a symbol like the colon operator, you have to use backticks (or quotes).
| This is so R knows you are not attempting to use the symbol in the command. Here's what it looks like: ?`:`.
                                                                                 | Don't forget the question mark out front.

> ?':'

| You got it!

  |=====================================                                                                    |  35%
| Often, we'll desire more control over a sequence we're creating than what the `:` operator gives us. The seq()
| function serves this purpose.

...

  |=========================================                                                                |  39%
| The most basic use of seq() does exactly the same thing as the `:` operator. Try seq(1, 20) to see this.

> seq(1, 20)
 [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20

| Perseverance, that's the answer.
                                                                                 
                                                                                 |==============================================                                                           |  43%
                                                                                 | This gives us the same output as 1:20. However, let's say that instead we want a vector of numbers ranging from
| 0 to 10, incremented by 0.5. seq(0, 10, by=0.5) does just that. Try it out.

> seq(0, 10, by = 0.5)
 [1]  0.0  0.5  1.0  1.5  2.0  2.5  3.0  3.5  4.0  4.5  5.0  5.5  6.0  6.5  7.0  7.5  8.0  8.5  9.0  9.5 10.0

| That's correct!
                                                                                   
                                                                                   |==================================================                                                       |  48%
                                                                                 | Or maybe we don't care what the increment is and we just want a sequence of 30 numbers between 5 and 10. seq(5,
| 10, length=30) does the trick. Give it a shot now and store the result in a new variable called my_seq.

> my_seq = seq(5, 10, length = 30)

| One more time. You can do it! Or, type info() for more options.

| You're using the same function here, but changing its arguments for different results. Be sure to store the
                                                                                 | result in a new variable called my_seq, like this: my_seq <- seq(5, 10, length=30).
                                                                                 
                                                                                 > my_seq <-  seq(5, 10, length = 30)
                                                                                 
                                                                                 | You got it!
                                                                                   
                                                                                   |=======================================================                                                  |  52%
                                                                                 | To confirm that my_seq has length 30, we can use the length() function. Try it now.
                                                                                 
                                                                                 > length(my_seq)
                                                                                 [1] 30
                                                                                 
                                                                                 | You got it!
                                                                                   
                                                                                   |===========================================================                                              |  57%
                                                                                 | Let's pretend we don't know the length of my_seq, but we want to generate a sequence of integers from 1 to N,
                                                                                 | where N represents the length of the my_seq vector. In other words, we want a new vector (1, 2, 3, ...) that is
                                                                                 | the same length as my_seq.
                                                                                 
                                                                                 ...
                                                                                 
                                                                                 |================================================================                                         |  61%
                                                                                 | There are several ways we could do this. One possibility is to combine the `:` operator and the length()
                                                                                 | function like this: 1:length(my_seq). Give that a try.
                                                                                 
                                                                                 > 1:length(my_seq)
                                                                                 [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30
                                                                                 
                                                                                 | Excellent job!
                                                                                   
                                                                                   |====================================================================                                     |  65%
                                                                                 | Another option is to use seq(along.with = my_seq). Give that a try.
                                                                                 
                                                                                 > seq(along.with = my_seq)
                                                                                 [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30
                                                                                 
                                                                                 | Your dedication is inspiring!
                                                                                   
                                                                                   |=========================================================================                                |  70%
                                                                                 | However, as is the case with many common tasks, R has a separate built-in function for this purpose called
                                                                                 | seq_along(). Type seq_along(my_seq) to see it in action.
                                                                                 
                                                                                 > seq_along(my_seq)
                                                                                 [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30
                                                                                 
                                                                                 | You're the best!

  |==============================================================================                           |  74%
| There are often several approaches to solving the same problem, particularly in R. Simple approaches that
| involve less typing are generally best. It's also important for your code to be readable, so that you and others
                                                                                 | can figure out what's going on without too much hassle.

...

  |==================================================================================                       |  78%
| If R has a built-in function for a particular task, it's likely that function is highly optimized for that
                                                                                 | purpose and is your best option. As you become a more advanced R programmer, you'll design your own functions to
| perform tasks when there are no better options. We'll explore writing your own functions in future lessons.
                                                                                 
                                                                                 ...
                                                                                 
                                                                                 |=======================================================================================                  |  83%
                                                                                 | One more function related to creating sequences of numbers is rep(), which stands for 'replicate'. Let's look at
| a few uses.

...

  |===========================================================================================              |  87%
| If we're interested in creating a vector that contains 40 zeros, we can use rep(0, times = 40). Try it out.
                                                                                 
                                                                                 > 
                                                                                   > rep(0, times = 40)
                                                                                 [1] 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
                                                                                 
                                                                                 | Excellent job!
                                                                                   
                                                                                   |================================================================================================         |  91%
                                                                                 | If instead we want our vector to contain 10 repetitions of the vector (0, 1, 2), we can do rep(c(0, 1, 2), times
                                                                                                                                                                                  | = 10). Go ahead.
                                                                                 
                                                                                 > rep(c(0, 1, 2), times = 1)
                                                                                 [1] 0 1 2
                                                                                 
                                                                                 | Not quite right, but keep trying. Or, type info() for more options.
                                                                                 
                                                                                 | Try rep(c(0, 1, 2), times = 10) for a different variation on the same theme. Be sure to use the c() function to
                                                                                 | tell R that the numbers 0, 1, and 2 make up a vector.
                                                                                 
                                                                                 > rep(c(0, 1, 2), times = 10)
                                                                                 [1] 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2
                                                                                 
                                                                                 | That's the answer I was looking for.

  |====================================================================================================     |  96%
| Finally, let's say that rather than repeating the vector (0, 1, 2) over and over again, we want our vector to
| contain 10 zeros, then 10 ones, then 10 twos. We can do this with the `each` argument. Try rep(c(0, 1, 2), each
                                                                                                                                                                                  | = 10).
> rep(c(0, 1, 2), each = 10)
[1] 0 0 0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 1 1 2 2 2 2 2 2 2 2 2 2
                                                                                 
| You are doing so well!
                                                                                   
                                                                                   |=========================================================================================================| 100%
 | Would you like to receive credit for completing this course on Coursera.org?
   1: Yes
 2: No
                                                                                 
 [1]   1  12 103   4
 Warning message:
   In c(1, 2, 3, 4) + c(0, 10, 100) :
   longer object length is not a multiple of shorter object length
 
 | Perseverance, that's the answer.

  |===========================================================================================              |  87%
| Before concluding this lesson, I'd like to show you a couple of time-saving tricks.
 
 ...
 
 |==============================================================================================           |  89%
 | Earlier in the lesson, you computed z * 2 + 100. Let's pretend that you made a mistake and that you meant to add
| 1000 instead of 100. You could either re-type the expression, or...

...

  |=================================================================================================        |  92%
| In many programming environments, the up arrow will cycle through previous commands. Try hitting the up arrow on
| your keyboard until you get to this command (z * 2 + 100), then change 100 to 1000 and hit Enter. If the up
| arrow doesn't work for you, just type the corrected command.
 
 > z * 2 + 1000
 [1] 1002.20 1018.00 1006.28
 
 | All that practice is paying off!
   
   |===================================================================================================      |  95%
 | Finally, let's pretend you'd like to view the contents of a variable that you created earlier, but you can't
| seem to remember if you named it my_div or myDiv. You could try both and see what works, or...

...

  |======================================================================================================   |  97%
| You can type the first two letters of the variable name, then hit the Tab key (possibly more than once). Most
| programming environments will provide a list of variables that you've created that begin with 'my'. This is
 | called auto-completion and can be quite handy when you have many variables in your workspace. Give it a try. (If
                                                                                                                 | auto-completion doesn't work for you, just type my_div and press Enter.)

> my_div
[1] 3.478505 3.181981 2.146460

| All that hard work is paying off!

  |=========================================================================================================| 100%
| Would you like to receive credit for completing this course on Coursera.org?

1: Yes
2: No

Selection: 2

| You are amazing!

| You've reached the end of this lesson! Returning to the main menu...
                                                                                                                 
                                                                                                                 | Please choose a course, or type 0 to exit swirl.
                                                                                                                 
                                                                                                                 1: R Programming
                                                                                                                 2: Take me to the swirl course repository!
                                                                                                                   
                                                                                                                   Selection: 1
                                                                                                                 
                                                                                                                 | Please choose a lesson, or type 0 to return to course menu.
                                                                                                                 
                                                                                                                 1: Basic Building Blocks      2: Workspace and Files        3: Sequences of Numbers    
                                                                                                                 4: Vectors                    5: Missing Values             6: Subsetting Vectors      
                                                                                                                 7: Matrices and Data Frames   8: Logic                      9: Functions               
                                                                                                                 10: lapply and sapply         11: vapply and tapply         12: Looking at Data         
                                                                                                                 13: Simulation                14: Dates and Times           15: Base Graphics           
                                                                                                                 
                                                                                                                 
                                                                                                                 Selection: 2
                                                                                                                 
                                                                                                                 |                                                                                                         |   0%
                                                                                                                 
                                                                                                                 | In this lesson, you'll learn how to examine your local workspace in R and begin to explore the relationship
| between your workspace and the file system of your machine.

...

  |===                                                                                                      |   3%
| Because different operating systems have different conventions with regards to things like file paths, the
| outputs of these commands may vary across machines.

...

  |=====                                                                                                    |   5%
| However it's important to note that R provides a common API (a common set of commands) for interacting with
                                                                                                                 | files, that way your code will work across different kinds of computers.
                                                                                                                 
                                                                                                                 ...
                                                                                                                 
                                                                                                                 |========                                                                                                 |   8%
                                                                                                                 | Let's jump right in so you can get a feel for how these special functions work!

...

  |===========                                                                                              |  10%
| Determine which directory your R session is using as its current working directory using getwd().

> getwd()
[1] "/Users/Claire/Desktop/Neurogenomics"

| You're the best!
                                                                                                                   
                                                                                                                   |=============                                                                                            |  13%
                                                                                                                 | List all the objects in your local workspace using ls().
                                                                                                                 
                                                                                                                 > ls()
                                                                                                                 [1] "my_div"  "my_sqrt" "x"       "y"       "z"      
                                                                                                                 
                                                                                                                 | That's a job well done!

  |================                                                                                         |  15%
| Some R commands are the same as their equivalents commands on Linux or on a Mac. Both Linux and Mac operating
| systems are based on an operating system called Unix. It's always a good idea to learn more about Unix!
                                                                                                                   
                                                                                                                   ...
                                                                                                                 
                                                                                                                 |===================                                                                                      |  18%
                                                                                                                 | Assign 9 to x using x <- 9.
                                                                                                                 
                                                                                                                 > x <- 9
                                                                                                                 
                                                                                                                 | You are quite good my friend!
                                                                                                                   
                                                                                                                   |======================                                                                                   |  21%
                                                                                                                 | Now take a look at objects that are in your workspace using ls().
                                                                                                                 
                                                                                                                 > ls()
                                                                                                                 [1] "my_div"  "my_sqrt" "x"       "y"       "z"      
                                                                                                                 
                                                                                                                 | All that hard work is paying off!
                                                                                                                   
                                                                                                                   |========================                                                                                 |  23%
                                                                                                                 | List all the files in your working directory using list.files() or dir().
                                                                                                                 
                                                                                                                 > list.files()
                                                                                                                 [1] "Neurogenomics.Rproj" "README.md"          
                                                                                                                 
                                                                                                                 | Your dedication is inspiring!
                                                                                                                   
                                                                                                                   |===========================                                                                              |  26%
                                                                                                                 | As we go through this lesson, you should be examining the help page for each new function. Check out the help
                                                                                                                 | page for list.files with the command ?list.files.
                                                                                                                 
                                                                                                                 > ?list.files
                                                                                                                 
                                                                                                                 | Your dedication is inspiring!
                                                                                                                   
                                                                                                                   |==============================                                                                           |  28%
                                                                                                                 | One of the most helpful parts of any R help file is the See Also section. Read that section for list.files. Some
                                                                                                                 | of these functions may be used in later portions of this lesson.
                                                                                                                 
                                                                                                                 ...
                                                                                                                 
                                                                                                                 |================================                                                                         |  31%
                                                                                                                 | Using the args() function on a function name is also a handy way to see what arguments a function can take.
                                                                                                                 
                                                                                                                 ...
                                                                                                                 
                                                                                                                 |===================================                                                                      |  33%
                                                                                                                 | Use the args() function to determine the arguments to list.files().
                                                                                                                 
                                                                                                                 > args(list.files)
                                                                                                                 function (path = ".", pattern = NULL, all.files = FALSE, full.names = FALSE, 
                                                                                                                           recursive = FALSE, ignore.case = FALSE, include.dirs = FALSE, 
                                                                                                                           no.. = FALSE) 
                                                                                                                   NULL
                                                                                                                 
                                                                                                                 | You are really on a roll!
                                                                                                                   
                                                                                                                   |======================================                                                                   |  36%
                                                                                                                 | Assign the value of the current working directory to a variable called "old.dir".
                                                                                                                 
                                                                                                                 > old.dir <- getwd()
                                                                                                                 
                                                                                                                 | You are quite good my friend!
                                                                                                                   
                                                                                                                   |========================================                                                                 |  38%
                                                                                                                 | We will use old.dir at the end of this lesson to move back to the place that we started. A lot of query
                                                                                                                 | functions like getwd() have the useful property that they return the answer to the question as a result of the
                                                                                                                 | function.
                                                                                                                 
                                                                                                                 ...
                                                                                                                 
                                                                                                                 |===========================================                                                              |  41%
                                                                                                                 | Use dir.create() to create a directory in the current working directory called "testdir".
                                                                                                                 
                                                                                                                 > dir.create()
                                                                                                                 Error in dir.create() : argument "path" is missing, with no default
                                                                                                                 > testdir = dir.create()
                                                                                                                 Error in dir.create() : argument "path" is missing, with no default
                                                                                                                 > dir.create()
                                                                                                                 Error in dir.create() : argument "path" is missing, with no default
                                                                                                                 > dir.create(testdir)
                                                                                                                 Error in dir.create(testdir) : object 'testdir' not found
                                                                                                                 > dir.create("testdir")
                                                                                                                 
                                                                                                                 | Excellent work!
                                                                                                                   
                                                                                                                   |==============================================                                                           |  44%
                                                                                                                 | We will do all our work in this new directory and then delete it after we are done. This is the R analog to
                                                                                                                 | "Take only pictures, leave only footprints."
                                                                                                                 
                                                                                                                 ...
                                                                                                                 
                                                                                                                 |================================================                                                         |  46%
                                                                                                                 | Set your working directory to "testdir" with the setwd() command.
                                                                                                                 
                                                                                                                 > setwd("testdir")
                                                                                                                 
                                                                                                                 | That's a job well done!

  |===================================================                                                      |  49%
| In general, you will want your working directory to be someplace sensible, perhaps created for the specific
| project that you are working on. In fact, organizing your work in R packages using RStudio is an excellent
| option. Check out RStudio at http://www.rstudio.com/

...

  |======================================================                                                   |  51%
| Create a file in your working directory called "mytest.R" using the file.create() function.

> file.create("mytest.R")
[1] TRUE

| All that hard work is paying off!

  |=========================================================                                                |  54%
| This should be the only file in this newly created directory. Let's check this by listing all the files in the
                                                                                                                 | current directory.
                                                                                                                 
                                                                                                                 > list.files()
                                                                                                                 [1] "mytest.R"
                                                                                                                 
                                                                                                                 | You're the best!

  |===========================================================                                              |  56%
| Check to see if "mytest.R" exists in the working directory using the file.exists() function.

> file.exists("mytest.R")
[1] TRUE

| You are amazing!

  |==============================================================                                           |  59%
| These sorts of functions are excessive for interactive use. But, if you are running a program that loops through
| a series of files and does some processing on each one, you will want to check to see that each exists before
| you try to process it.

...

  |=================================================================                                        |  62%
| Access information about the file "mytest.R" by using file.info().

> file.infor("mytest.R")
Error in file.infor("mytest.R") : could not find function "file.infor"
> file.info("mytest.R")
         size isdir mode               mtime               ctime               atime uid gid  uname grname
mytest.R    0 FALSE  644 2019-09-20 12:32:54 2019-09-20 12:32:54 2019-09-20 12:32:56 502  20 Claire  staff

| You nailed it! Good job!

  |===================================================================                                      |  64%
| You can use the $ operator --- e.g., file.info("mytest.R")$mode --- to grab specific items.

...

  |======================================================================                                   |  67%
| Change the name of the file "mytest.R" to "mytest2.R" by using file.rename().

> file.rename("mytest2.R")
Error in file.rename("mytest2.R") : 
  argument "to" is missing, with no default
> file.rename("mytest.3", "mytest2.R")
[1] FALSE
Warning message:
In file.rename("mytest.3", "mytest2.R") :
  cannot rename file 'mytest.3' to 'mytest2.R', reason 'No such file or directory'

| Keep trying! Or, type info() for more options.

| file.rename("mytest.R", "mytest2.R") is the answer. Googling using key words from the question, along with the
| letter R, will often give you a good hint.

> file.rename("mytest.R", "mytest2.R")
[1] TRUE

| Excellent work!

  |=========================================================================                                |  69%
| Your operating system will provide simpler tools for these sorts of tasks, but having the ability to manipulate
| files programatically is useful. You might now try to delete mytest.R using file.remove('mytest.R'), but that
| won't work since mytest.R no longer exists. You have already renamed it.
                                                                                                                 
                                                                                                                 ...
                                                                                                                 
                                                                                                                 |===========================================================================                              |  72%
                                                                                                                 | Make a copy of "mytest2.R" called "mytest3.R" using file.copy().
                                                                                                                 
                                                                                                                 > file.copy(mytest2.R, mytest3.R)
                                                                                                                 Error in file.copy(mytest2.R, mytest3.R) : object 'mytest2.R' not found
                                                                                                                 > list.files()
                                                                                                                 [1] "mytest2.R"
                                                                                                                 
                                                                                                                 | You're close...I can feel it! Try it again. Or, type info() for more options.

| file.copy("mytest2.R", "mytest3.R") works.

> file.copy("mytest2.R", "mytest3.R" )
[1] TRUE

| That's the answer I was looking for.
                                                                                                                 
                                                                                                                 |==============================================================================                           |  74%
                                                                                                                 | You now have two files in the current directory. That may not seem very interesting. But what if you were
                                                                                                                 | working with dozens, or millions, of individual files? In that case, being able to programatically act on many
                                                                                                                 | files would be absolutely necessary. Don't forget that you can, temporarily, leave the lesson by typing play()
| and then return by typing nxt().

...

  |=================================================================================                        |  77%
| Provide the relative path to the file "mytest3.R" by using file.path().

> file.path("mytest3.R")
[1] "mytest3.R"

| All that hard work is paying off!

  |===================================================================================                      |  79%
| You can use file.path to construct file and directory paths that are independent of the operating system your R
| code is running on. Pass 'folder1' and 'folder2' as arguments to file.path to make a platform-independent
| pathname.

> file.path('folder1', 'folder2')
[1] "folder1/folder2"

| You got it right!

  |======================================================================================                   |  82%
| Take a look at the documentation for dir.create by entering ?dir.create . Notice the 'recursive' argument. In
| order to create nested directories, 'recursive' must be set to TRUE.

> ?dir.create

| Keep working like that and you'll get there!
                                                                                                                   
                                                                                                                   |=========================================================================================                |  85%
                                                                                                                 | Create a directory in the current working directory called "testdir2" and a subdirectory for it called
                                                                                                                 | "testdir3", all in one command by using dir.create() and file.path().
                                                                                                                 
                                                                                                                 > file.path(dir.create("testdir2"), dir.create("testdir3"))
                                                                                                                 [1] "TRUE/TRUE"
                                                                                                                 
                                                                                                                 | That's not the answer I was looking for, but try again. Or, type info() for more options.

| dir.create(file.path('testdir2', 'testdir3'), recursive = TRUE) will do the trick. If you forgot the recursive
| argument, the command may have appeared to work, but it didn't create the nested directory.
                                                                                                                 
                                                                                                                 > dir.create(file.path("testdir2","testdir3"), recursive = TRUE)
                                                                                                                 
                                                                                                                 | You got it!
                                                                                                                   
                                                                                                                   |============================================================================================             |  87%
                                                                                                                 | Go back to your original working directory using setwd(). (Recall that we created the variable old.dir with the
                                                                                                                                                                              | full path for the orginal working directory at the start of these questions.)
                                                                                                                 
                                                                                                                 > setwd(old.dir)
                                                                                                                 
                                                                                                                 | You got it!
                                                                                                                   
                                                                                                                   |==============================================================================================           |  90%
                                                                                                                 | It is often helpful to save the settings that you had before you began an analysis and then go back to them at
                                                                                                                 | the end. This trick is often used within functions; you save, say, the par() settings that you started with,
                                                                                                                 | mess around a bunch, and then set them back to the original values at the end. This isn't the same as what we
| have done here, but it seems similar enough to mention.

...

  |=================================================================================================        |  92%
| After you finish this lesson delete the 'testdir' directory that you just left (and everything in it)

...

  |====================================================================================================     |  95%
| Take nothing but results. Leave nothing but assumptions. That sounds like 'Take nothing but pictures. Leave
                                                                                                                 | nothing but footprints.' But it makes no sense! Surely our readers can come up with a better motto . . .

...

  |======================================================================================================   |  97%
| In this lesson, you learned how to examine your R workspace and work with the file system of your machine from
| within R. Thanks for playing!

...

  |=========================================================================================================| 100%
| Would you like to receive credit for completing this course on Coursera.org?

1: No
2: Yes

Selection: y
Enter an item from the menu, or 0 to exit
Selection: 2
What is your email address? claireeverett11@gmail.com
What is your assignment token? 


| Leaving swirl now. Type swirl() to resume.

> swirl()

| Welcome to swirl! Please sign in. If you've been here before, use the same name as you did then. If you are new,
                                                                                                                 | call yourself something unique.
                                                                                                                 
                                                                                                                 What shall I call you? Claire
                                                                                                                 
                                                                                                                 | Would you like to continue with one of these lessons?
                                                                                                                   
                                                                                                                   1: R Programming Workspace and Files
                                                                                                                 2: No. Let me start something new.
                                                                                                                 
                                                                                                                 Selection: 1
                                                                                                                 
                                                                                                                 
                                                                                                                 
                                                                                                                 | Would you like to receive credit for completing this course on Coursera.org?
                                                                                                                   
                                                                                                                   1: Yes
                                                                                                                 2: No
                                                                                                                 
                                                                                                                 Selection: 2
                                                                                                                 
                                                                                                                 | That's the answer I was looking for.

| You've reached the end of this lesson! Returning to the main menu...
                                                                                                                 
                                                                                                                 | Please choose a course, or type 0 to exit swirl.
                                                                                                                 
                                                                                                                 1: R Programming
                                                                                                                 2: Take me to the swirl course repository!
                                                                                                                   
                                                                                                                   Selection: 1
                                                                                                                 
                                                                                                                 | Please choose a lesson, or type 0 to return to course menu.
                                                                                                                 
                                                                                                                 1: Basic Building Blocks      2: Workspace and Files        3: Sequences of Numbers    
                                                                                                                 4: Vectors                    5: Missing Values             6: Subsetting Vectors      
                                                                                                                 7: Matrices and Data Frames   8: Logic                      9: Functions               
                                                                                                                 10: lapply and sapply         11: vapply and tapply         12: Looking at Data         
                                                                                                                 13: Simulation                14: Dates and Times           15: Base Graphics           
                                                                                                                 
                                                                                                                 
                                                                                                                 Selection: 3
                                                                                                                 
                                                                                                                 |                                                                                                         |   0%
                                                                                                                 
                                                                                                                 | In this lesson, you'll learn how to create sequences of numbers in R.

...

  |=====                                                                                                    |   4%
| The simplest way to create a sequence of numbers in R is by using the `:` operator. Type 1:20 to see how it
| works.

> 1:20
 [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20

| You are amazing!

  |=========                                                                                                |   9%
| That gave us every integer between (and including) 1 and 20. We could also use it to create a sequence of real
| numbers. For example, try pi:10.

> pi:10
[1] 3.141593 4.141593 5.141593 6.141593 7.141593 8.141593 9.141593

| Nice work!

  |==============                                                                                           |  13%
| The result is a vector of real numbers starting with pi (3.142...) and increasing in increments of 1. The upper
| limit of 10 is never reached, since the next number in our sequence would be greater than 10.

...

  |==================                                                                                       |  17%
| What happens if we do 15:1? Give it a try to find out.

> 15:1
 [1] 15 14 13 12 11 10  9  8  7  6  5  4  3  2  1

| Perseverance, that's the answer.
                                                                                                                 
                                                                                                                 |=======================                                                                                  |  22%
                                                                                                                 | It counted backwards in increments of 1! It's unlikely we'd want this behavior, but nonetheless it's good to
| know how it could happen.

...

  |===========================                                                                              |  26%
| Remember that if you have questions about a particular R function, you can access its documentation with a
| question mark followed by the function name: ?function_name_here. However, in the case of an operator like the
| colon used above, you must enclose the symbol in backticks like this: ?`:`. (NOTE: The backtick (`) key is
| generally located in the top left corner of a keyboard, above the Tab key. If you don't have a backtick key, you
                                                                                                                 | can use regular quotes.)
 
 ...
 
 |================================                                                                         |  30%
 | Pull up the documentation for `:` now.
 
 > help(':')
 
 | You almost had it, but not quite. Try again. Or, type info() for more options.
 
 | In order to view the documentation for a symbol like the colon operator, you have to use backticks (or quotes).
 | This is so R knows you are not attempting to use the symbol in the command. Here's what it looks like: ?`:`.
| Don't forget the question mark out front.
 
 > ':'
 [1] ":"
 
 | Keep trying! Or, type info() for more options.
 
 | In order to view the documentation for a symbol like the colon operator, you have to use backticks (or quotes).
 | This is so R knows you are not attempting to use the symbol in the command. Here's what it looks like: ?`:`.
| Don't forget the question mark out front.
 
 > ?':'
 
 | You got it!
   
   |=====================================                                                                    |  35%
 | Often, we'll desire more control over a sequence we're creating than what the `:` operator gives us. The seq()
 | function serves this purpose.
 
 ...
 
 |=========================================                                                                |  39%
 | The most basic use of seq() does exactly the same thing as the `:` operator. Try seq(1, 20) to see this.
 
 > seq(1, 20)
 [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20
 
 | Perseverance, that's the answer.

  |==============================================                                                           |  43%
| This gives us the same output as 1:20. However, let's say that instead we want a vector of numbers ranging from
 | 0 to 10, incremented by 0.5. seq(0, 10, by=0.5) does just that. Try it out.
 
 > seq(0, 10, by = 0.5)
 [1]  0.0  0.5  1.0  1.5  2.0  2.5  3.0  3.5  4.0  4.5  5.0  5.5  6.0  6.5  7.0  7.5  8.0  8.5  9.0  9.5 10.0
 
 | That's correct!

  |==================================================                                                       |  48%
| Or maybe we don't care what the increment is and we just want a sequence of 30 numbers between 5 and 10. seq(5,
                                                                                                               | 10, length=30) does the trick. Give it a shot now and store the result in a new variable called my_seq.
 
 > my_seq = seq(5, 10, length = 30)
 
 | One more time. You can do it! Or, type info() for more options.
 
 | You're using the same function here, but changing its arguments for different results. Be sure to store the
| result in a new variable called my_seq, like this: my_seq <- seq(5, 10, length=30).

> my_seq <-  seq(5, 10, length = 30)

| You got it!

  |=======================================================                                                  |  52%
| To confirm that my_seq has length 30, we can use the length() function. Try it now.

> length(my_seq)
[1] 30

| You got it!

  |===========================================================                                              |  57%
| Let's pretend we don't know the length of my_seq, but we want to generate a sequence of integers from 1 to N,
| where N represents the length of the my_seq vector. In other words, we want a new vector (1, 2, 3, ...) that is
| the same length as my_seq.

...

  |================================================================                                         |  61%
| There are several ways we could do this. One possibility is to combine the `:` operator and the length()
| function like this: 1:length(my_seq). Give that a try.

> 1:length(my_seq)
 [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30

| Excellent job!

  |====================================================================                                     |  65%
| Another option is to use seq(along.with = my_seq). Give that a try.

> seq(along.with = my_seq)
 [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30

| Your dedication is inspiring!

  |=========================================================================                                |  70%
| However, as is the case with many common tasks, R has a separate built-in function for this purpose called
| seq_along(). Type seq_along(my_seq) to see it in action.

> seq_along(my_seq)
 [1]  1  2  3  4  5  6  7  8  9 10 11 12 13 14 15 16 17 18 19 20 21 22 23 24 25 26 27 28 29 30

| You're the best!
   
   |==============================================================================                           |  74%
 | There are often several approaches to solving the same problem, particularly in R. Simple approaches that
 | involve less typing are generally best. It's also important for your code to be readable, so that you and others
| can figure out what's going on without too much hassle.
 
 ...
 
 |==================================================================================                       |  78%
 | If R has a built-in function for a particular task, it's likely that function is highly optimized for that
| purpose and is your best option. As you become a more advanced R programmer, you'll design your own functions to
 | perform tasks when there are no better options. We'll explore writing your own functions in future lessons.

...

  |=======================================================================================                  |  83%
| One more function related to creating sequences of numbers is rep(), which stands for 'replicate'. Let's look at
 | a few uses.
 
 ...
 
 |===========================================================================================              |  87%
 | If we're interested in creating a vector that contains 40 zeros, we can use rep(0, times = 40). Try it out.

> 
> rep(0, times = 40)
 [1] 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0

| Excellent job!

  |================================================================================================         |  91%
| If instead we want our vector to contain 10 repetitions of the vector (0, 1, 2), we can do rep(c(0, 1, 2), times
| = 10). Go ahead.

> rep(c(0, 1, 2), times = 1)
[1] 0 1 2

| Not quite right, but keep trying. Or, type info() for more options.

| Try rep(c(0, 1, 2), times = 10) for a different variation on the same theme. Be sure to use the c() function to
| tell R that the numbers 0, 1, and 2 make up a vector.

> rep(c(0, 1, 2), times = 10)
 [1] 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2 0 1 2

| That's the answer I was looking for.
 
 |====================================================================================================     |  96%
 | Finally, let's say that rather than repeating the vector (0, 1, 2) over and over again, we want our vector to
| contain 10 zeros, then 10 ones, then 10 twos. We can do this with the `each` argument. Try rep(c(0, 1, 2), each
| = 10).

> rep(c(0, 1, 2), each = 10)
 [1] 0 0 0 0 0 0 0 0 0 0 1 1 1 1 1 1 1 1 1 1 2 2 2 2 2 2 2 2 2 2

| You are doing so well!

  |=========================================================================================================| 100%
| Would you like to receive credit for completing this course on Coursera.org?

1: Yes
2: No

Selection: 2

| You got it!

| You've reached the end of this lesson! Returning to the main menu...
 
 | Please choose a course, or type 0 to exit swirl.
 
 1: R Programming
 2: Take me to the swirl course repository!
   
   Selection: 1
 
 | Please choose a lesson, or type 0 to return to course menu.
 
 1: Basic Building Blocks      2: Workspace and Files        3: Sequences of Numbers    
 4: Vectors                    5: Missing Values             6: Subsetting Vectors      
 7: Matrices and Data Frames   8: Logic                      9: Functions               
 10: lapply and sapply         11: vapply and tapply         12: Looking at Data         
 13: Simulation                14: Dates and Times           15: Base Graphics           
 
 
 Selection: 4
 
 |                                                                                                         |   0%
 
 | The simplest and most common data structure in R is the vector.
 
 ...
 
 |===                                                                                                      |   3%
 | Vectors come in two different flavors: atomic vectors and lists. An atomic vector contains exactly one data
 | type, whereas a list may contain multiple data types. We'll explore atomic vectors further before we get to
| lists.

...

  |======                                                                                                   |   5%
| In previous lessons, we dealt entirely with numeric vectors, which are one type of atomic vector. Other types of
| atomic vectors include logical, character, integer, and complex. In this lesson, we'll take a closer look at
 | logical and character vectors.
 
 ...
 
 |========                                                                                                 |   8%
 | Logical vectors can contain the values TRUE, FALSE, and NA (for 'not available'). These values are generated as
 | the result of logical 'conditions'. Let's experiment with some simple conditions.

...

  |===========                                                                                              |  11%
| First, create a numeric vector num_vect that contains the values 0.5, 55, -10, and 6.

> num_vect <- c(0.5, 55, -10, 6)

| You got it!

  |==============                                                                                           |  13%
| Now, create a variable called tf that gets the result of num_vect < 1, which is read as 'num_vect is less than
 | 1'.

> tf <- num_vect < 1

| Excellent work!

  |=================                                                                                        |  16%
| What do you think tf will look like?

1: a single logical value
2: a vector of 4 logical values

Selection: 2

| Nice work!

  |===================                                                                                      |  18%
| Print the contents of tf now.

> tf
[1]  TRUE FALSE  TRUE FALSE

| You nailed it! Good job!

  |======================                                                                                   |  21%
| The statement num_vect < 1 is a condition and tf tells us whether each corresponding element of our numeric
| vector num_vect satisfies this condition.

...

  |=========================                                                                                |  24%
| The first element of num_vect is 0.5, which is less than 1 and therefore the statement 0.5 < 1 is TRUE. The
| second element of num_vect is 55, which is greater than 1, so the statement 55 < 1 is FALSE. The same logic
| applies for the third and fourth elements.

...

  |============================                                                                             |  26%
| Let's try another. Type num_vect >= 6 without assigning the result to a new variable.
 
 > num_vect >= 6
 [1] FALSE  TRUE FALSE  TRUE
 
 | That's correct!

  |==============================                                                                           |  29%
| This time, we are asking whether each individual element of num_vect is greater than OR equal to 6. Since only
| 55 and 6 are greater than or equal to 6, the second and fourth elements of the result are TRUE and the first and
| third elements are FALSE.

...

  |=================================                                                                        |  32%
| The `<` and `>=` symbols in these examples are called 'logical operators'. Other logical operators include `>`,
| `<=`, `==` for exact equality, and `!=` for inequality.

...

  |====================================                                                                     |  34%
| If we have two logical expressions, A and B, we can ask whether at least one is TRUE with A | B (logical 'or'
| a.k.a. 'union') or whether they are both TRUE with A & B (logical 'and' a.k.a. 'intersection'). Lastly, !A is
| the negation of A and is TRUE when A is FALSE and vice versa.

...

  |=======================================                                                                  |  37%
| It's a good idea to spend some time playing around with various combinations of these logical operators until
 | you get comfortable with their use. We'll do a few examples here to get you started.

...

  |=========================================                                                                |  39%
| Try your best to predict the result of each of the following statements. You can use pencil and paper to work
| them out if it's helpful. If you get stuck, just guess and you've got a 50% chance of getting the right answer!

...

  |============================================                                                             |  42%
| (3 > 5) & (4 == 4)

1: TRUE
2: FALSE

Selection: 2

| Great job!

  |===============================================                                                          |  45%
| (TRUE == TRUE) | (TRUE == FALSE)

1: TRUE
2: FALSE

Selection: 1

| You are quite good my friend!

  |==================================================                                                       |  47%
| ((111 >= 111) | !(TRUE)) & ((4 + 1) == 5)

1: TRUE
2: FALSE

Selection: 1

| You are quite good my friend!

  |====================================================                                                     |  50%
| Don't worry if you found these to be tricky. They're supposed to be. Working with logical statements in R takes
| practice, but your efforts will be rewarded in future lessons (e.g. subsetting and control structures).

...

  |=======================================================                                                  |  53%
| Character vectors are also very common in R. Double quotes are used to distinguish character objects, as in the
| following example.

...

  |==========================================================                                               |  55%
| Create a character vector that contains the following words: "My", "name", "is". Remember to enclose each word
| in its own set of double quotes, so that R knows they are character strings. Store the vector in a variable
| called my_char.

> 
> my_char <- c("My", "name", "is")

| Keep working like that and you'll get there!
   
   |=============================================================                                            |  58%
 | Print the contents of my_char to see what it looks like.
 
 > my_char
 [1] "My"   "name" "is"  
 
 | You nailed it! Good job!
   
   |================================================================                                         |  61%
 | Right now, my_char is a character vector of length 3. Let's say we want to join the elements of my_char together
| into one continuous character string (i.e. a character vector of length 1). We can do this using the paste()
| function.

...

  |==================================================================                                       |  63%
| Type paste(my_char, collapse = " ") now. Make sure there's a space between the double quotes in the `collapse`
 | argument. You'll see why in a second.

> paste(my_char, collapse = " ")
[1] "My name is"

| You got it!

  |=====================================================================                                    |  66%
| The `collapse` argument to the paste() function tells R that when we join together the elements of the my_char
| character vector, we'd like to separate them with single spaces.
 
 ...
 
 |========================================================================                                 |  68%
 | It seems that we're missing something.... Ah, yes! Your name!

...

  |===========================================================================                              |  71%
| To add (or 'concatenate') your name to the end of my_char, use the c() function like this: c(my_char,
| "your_name_here"). Place your name in double quotes where I've put "your_name_here". Try it now, storing the
 | result in a new variable called my_name.
 
 > c(my_char, "Claire")
 [1] "My"     "name"   "is"     "Claire"
 
 | You almost had it, but not quite. Try again. Or, type info() for more options.
 
 | Tack your name on to the end of the my_char vector using the c() function.  Be sure to assign the result to a
 | new variable called my_name. If your name was "Swirl", you would type my_name <- c(my_char, "Swirl").
 
 > my_name <- c(my_char, "Claire")
 
 | Excellent work!
   
   |=============================================================================                            |  74%
 | Take a look at the contents of my_name.
 
 > my_name
 [1] "My"     "name"   "is"     "Claire"
 
 | Keep working like that and you'll get there!

  |================================================================================                         |  76%
| Now, use the paste() function once more to join the words in my_name together into a single character string.
| Don't forget to say collapse = " "!
   
   > paste(my_name, collapse = " ")
 [1] "My name is Claire"
 
 | You nailed it! Good job!
   
   |===================================================================================                      |  79%
 | In this example, we used the paste() function to collapse the elements of a single character vector. paste() can
 | also be used to join the elements of multiple character vectors.
 
 ...
 
 |======================================================================================                   |  82%
 | In the simplest case, we can join two character vectors that are each of length 1 (i.e. join two words). Try
 | paste("Hello", "world!", sep = " "), where the `sep` argument tells R that we want to separate the joined
 | elements with a single space.
 
 > paste("Hello", "world!", sep = " ")
 [1] "Hello world!"
 
 | You're the best!

  |========================================================================================                 |  84%
| For a slightly more complicated example, we can join two vectors, each of length 3. Use paste() to join the
| integer vector 1:3 with the character vector c("X", "Y", "Z"). This time, use sep = "" to leave no space between
| the joined elements.

> paste(1:3, c("X", "Y", "Z"), sep = "")
[1] "1X" "2Y" "3Z"

| Your dedication is inspiring!

  |===========================================================================================              |  87%
| What do you think will happen if our vectors are of different length? (Hint: we talked about this in a previous
| lesson.)

...

  |==============================================================================================           |  89%
| Vector recycling! Try paste(LETTERS, 1:4, sep = "-"), where LETTERS is a predefined variable in R containing a
| character vector of all 26 letters in the English alphabet.

> paste(LETTERS, 1:4, sep = "-")
 [1] "A-1" "B-2" "C-3" "D-4" "E-1" "F-2" "G-3" "H-4" "I-1" "J-2" "K-3" "L-4" "M-1" "N-2" "O-3" "P-4" "Q-1" "R-2"
[19] "S-3" "T-4" "U-1" "V-2" "W-3" "X-4" "Y-1" "Z-2"

| That's correct!
   
   |=================================================================================================        |  92%
 | Since the character vector LETTERS is longer than the numeric vector 1:4, R simply recycles, or repeats, 1:4
 | until it matches the length of LETTERS.
 
 ...
 
 |===================================================================================================      |  95%
 | Also worth noting is that the numeric vector 1:4 gets 'coerced' into a character vector by the paste() function.
 
 ...
 
 |======================================================================================================   |  97%
 | We'll discuss coercion in another lesson, but all it really means is that the numbers 1, 2, 3, and 4 in the
| output above are no longer numbers to R, but rather characters "1", "2", "3", and "4".

...

  |=========================================================================================================| 100%
| Would you like to receive credit for completing this course on Coursera.org?

1: Yes
2: No

 1: Basic Building Blocks      2: Workspace and Files        3: Sequences of Numbers    
 4: Vectors                    5: Missing Values             6: Subsetting Vectors      
 7: Matrices and Data Frames   8: Logic                      9: Functions               
10: lapply and sapply         11: vapply and tapply         12: Looking at Data         
13: Simulation                14: Dates and Times           15: Base Graphics           


Selection: 5

  |                                                                                                         |   0%

| Missing values play an important role in statistics and data analysis. Often, missing values must not be
| ignored, but rather they should be carefully studied to see if there's an underlying pattern or cause for their
 | missingness.
 
 ...
 
 |=====                                                                                                    |   5%
 | In R, NA is used to represent any value that is 'not available' or 'missing' (in the statistical sense). In this
 | lesson, we'll explore missing values further.

...

  |==========                                                                                               |  10%
| Any operation involving NA generally yields NA as the result. To
| illustrate, let's create a vector c(44, NA, 5, NA) and assign it to a
 | variable x.
 
 > x <-  c(44, NA, 5, NA)
 
 | Excellent work!
   
   |================                                                                                         |  15%
 | Now, let's multiply x by 3.

> x *3
[1] 132  NA  15  NA

| Great job!

  |=====================                                                                                    |  20%
| Notice that the elements of the resulting vector that correspond with the NA values in x are also NA.

...

  |==========================                                                                               |  25%
| To make things a little more interesting, lets create a vector containing 1000 draws from a standard normal
| distribution with y <- rnorm(1000).

> y <- rnorm(1000)

| Excellent work!

  |================================                                                                         |  30%
| Next, let's create a vector containing 1000 NAs with z <- rep(NA, 1000).
 
 > z <-  rep(NA, 1000)
 
 | Nice work!
   
   |=====================================                                                                    |  35%
 | Finally, let's select 100 elements at random from these 2000 values (combining y and z) such that we don't know
 | how many NAs we'll wind up with or what positions they'll occupy in our final vector -- my_data <- sample(c(y,
                                                                                                               | z), 100).
 
 > my_data <- sample(c(y,z), 100)
 
 | That's a job well done!

  |==========================================                                                               |  40%
| Let's first ask the question of where our NAs are located in our data. The is.na() function tells us whether
 | each element of a vector is NA. Call is.na() on my_data and assign the result to my_na.
 
 > my_na = is.na(my_data)
 
 | Not quite, but you're learning! Try again. Or, type info() for more options.

| Assign the result of is.na(my_data) to the variable my_na.

> my_na <-  is.na(my_data)

| You got it!

  |===============================================                                                          |  45%
| Now, print my_na to see what you came up with.

> my_na
  [1]  TRUE FALSE  TRUE  TRUE FALSE FALSE FALSE  TRUE  TRUE FALSE FALSE  TRUE  TRUE  TRUE  TRUE  TRUE FALSE  TRUE
 [19] FALSE FALSE FALSE FALSE FALSE  TRUE FALSE FALSE FALSE FALSE FALSE  TRUE  TRUE  TRUE  TRUE FALSE FALSE FALSE
 [37]  TRUE  TRUE FALSE  TRUE FALSE  TRUE FALSE  TRUE FALSE FALSE  TRUE FALSE  TRUE  TRUE  TRUE  TRUE  TRUE FALSE
 [55]  TRUE FALSE FALSE  TRUE FALSE  TRUE FALSE FALSE FALSE  TRUE  TRUE  TRUE FALSE FALSE FALSE  TRUE FALSE FALSE
 [73]  TRUE  TRUE  TRUE FALSE  TRUE  TRUE FALSE  TRUE  TRUE FALSE FALSE  TRUE FALSE FALSE  TRUE FALSE  TRUE FALSE
 [91]  TRUE  TRUE  TRUE FALSE  TRUE FALSE FALSE  TRUE FALSE FALSE

| You're the best!
   
   |====================================================                                                     |  50%
 | Everywhere you see a TRUE, you know the corresponding element of my_data is NA. Likewise, everywhere you see a
 | FALSE, you know the corresponding element of my_data is one of our random draws from the standard normal
 | distribution.
 
 ...
 
 |==========================================================                                               |  55%
 | In our previous discussion of logical operators, we introduced the `==` operator as a method of testing for
 | equality between two objects. So, you might think the expression my_data == NA yields the same results as
 | is.na(). Give it a try.
 
 > my_data == NA
 [1] NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA
 [37] NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA
 [73] NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA NA
 
 | All that hard work is paying off!
   
   |===============================================================                                          |  60%
 | The reason you got a vector of all NAs is that NA is not really a value, but just a placeholder for a quantity
 | that is not available. Therefore the logical expression is incomplete and R has no choice but to return a vector
 | of the same length as my_data that contains all NAs.
 
 ...
 
 |====================================================================                                     |  65%
 | Don't worry if that's a little confusing. The key takeaway is to be cautious when using logical expressions
 | anytime NAs might creep in, since a single NA value can derail the entire thing.
 
 ...
 
 |==========================================================================                               |  70%
 | So, back to the task at hand. Now that we have a vector, my_na, that has a TRUE for every NA and FALSE for every
 | numeric value, we can compute the total number of NAs in our data.
 
 ...
 
 |===============================================================================                          |  75%
 | The trick is to recognize that underneath the surface, R represents TRUE as the number 1 and FALSE as the number
 | 0. Therefore, if we take the sum of a bunch of TRUEs and FALSEs, we get the total number of TRUEs.
 
 ...
 
 |====================================================================================                     |  80%
 | Let's give that a try here. Call the sum() function on my_na to count the total number of TRUEs in my_na, and
| thus the total number of NAs in my_data. Don't assign the result to a new variable.
 
 > sum(my_na)
 [1] 49
 
 | Perseverance, that's the answer.

  |=========================================================================================                |  85%
| Pretty cool, huh? Finally, let's take a look at the data to convince ourselves that everything 'adds up'. Print
 | my_data to the console.
 
 > my_data
 [1]           NA -1.848109404           NA           NA -0.594481914 -0.482599965  1.171942866           NA
 [9]           NA -0.903638025 -0.331481730           NA           NA           NA           NA           NA
 [17]  0.356165445           NA  0.266085890  0.740870954 -1.195909992  1.211330946  0.764245446           NA
 [25] -1.274774949  0.079592421 -1.480841201 -0.105022562  0.699693329           NA           NA           NA
 [33]           NA  0.332342473  0.001389168 -0.403646476           NA           NA  0.783136173           NA
 [41]  0.627111041           NA  0.675453645           NA  0.688529770 -0.846301055           NA -0.543074589
 [49]           NA           NA           NA           NA           NA -0.579832453           NA -0.287516056
 [57] -0.962381943           NA -0.173883172           NA  0.952203909  1.156778229  0.540600210           NA
 [65]           NA           NA  0.024984304  1.398976064 -1.108590076           NA  0.975785413  2.023992139
 [73]           NA           NA           NA  0.820506220           NA           NA  0.201601284           NA
 [81]           NA -0.557450936 -0.570122887           NA -2.283281596  0.027011464           NA  0.448180489
 [89]           NA  0.974066664           NA           NA           NA -0.174015454           NA -1.266655707
 [97] -1.176068163           NA -0.760162029  0.331039529
 
 | Perseverance, that's the answer.

  |==============================================================================================           |  90%
| Now that we've got NAs down pat, let's look at a second type of missing value -- NaN, which stands for 'not a
 | number'. To generate NaN, try dividing (using a forward slash) 0 by 0 now.

> 0/0
[1] NaN

| You nailed it! Good job!

  |====================================================================================================     |  95%
| Let's do one more, just for fun. In R, Inf stands for infinity. What happens if you subtract Inf from Inf?
   
   > Inf - Inf
 [1] NaN
 
 | All that hard work is paying off!
   
   |=========================================================================================================| 100%
 | Would you like to receive credit for completing this course on Coursera.org?
   
   1: No
 2: Yes
 
 Selection: 
