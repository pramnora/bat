# bat
MS DOS/Microsoft Disk Operating System batch files: [.bat]

## MS DOS Batch file programming history

Before the Windows OS/Operating System was invented...which uses the WIMP/Window Icons Mouse Pointer...or, GUI/Graphical User Interface system; there was the MS DOS CLI/Command Line Interface operating system, instead; and, this is just a 'black' screen...which also contains what is known as a MS DOS 'Command prompt' symbol.

C:\>

...and, the user would type in command instructions after the prompt.

C:\> DIR

...the above DIR instruction, for example would show the current directory listing of files/folders/-etc.

**NOTE:** The MS DOS Command prompt symbol should read as: C + colon + backwards slash + right pointing chevron/arrow; however, MarkDown (.md) is not allowing the display of the 'backwards slash'...?!   

## How to get help on how to use any MS DOS Command

In order to get help on how to use any MS DOS COMMAND...

C:\> DIR /?

...that is, DIR + space + forwards slash + question mark...; then, press the [ENTER] key...; will display a list of further instructions on how to use the command.

## The use of MS DOS command switches - used to modify the commands output

If say a DIR listing is especially long...; then, you might wish to use the /P switch...which displays the data just one single page at a time...(otherwise, the long directory listing might scroll down so 'fast' that you can't actually see/read it?!)

C:\> DIR /? /P

...the /P switch will state at the bottom of the page...press any key to continue; then, go on to show the next page...and, so on...until the end of the file is reached.

**NOTE:** Each MS DOS Command has it's own entirely 'unique' series of switches.

## Batch program files

There are 2 ways to run MS DOS Commands...

1. 'Interactively', by typing in the commands inside of the MS DOS Command prompt window

In order to open up an MS DOS Command prompt window...  

a -  DO a combination key press: [WINDOWS PICTURE ICON KEY]+[R]...and, a Run dialog box should appear  

b - Type into the Run dialog box: CMD...and, then, press the [OK] button...  
    this should make the 'black' screen MS DOS prompt window appear ready for typing command instructions into  

c - Type: ECHO hello, world...and, press the [ENTER] key...and the words: 'hello, world' will show.  

d - In order to close the MS DOS black screen window...either type: EXIT...then, press [ENTER] key/or else, hit the windows top right [x].  

2. 'Programmatically', -also, known as 'silent' mode-, by including the commands inside of what is known as a batch program file.

(Instructions are shown below.)

## What are batch [.bat] file programs?

First, a program file is nothing more than a plain text file: [filename.txt]...; which has been saved using a special filename extension: [.bat].

A batch file program uses: [filename.bat].

a. Where the [filename] part can be any filename you please.

b. The 3 letter filename exension: [.bat] is what turns the otherwise ordinary plain text file: [.txt] into becoming a batch file program, instead.

Batch files contain a list of instructions...MS DOS Commands...which are executed using 'top down flow'...whenever the program runs/executes.

## How to create a batch file program/and, make it execute...

1. Open Windows Notepad word processor program

a. Do a combination key press: [WINDOWS PICTURE ICON KEY]+[R]...and, the Run dialog box should open...

b. Type in to the Run dialog box: Notepad...and, press the [OK] button...should make a Notepad window appear...;  
   ready for typing futher instructions into.

2. Type into the Notepad screen...the following 3 lines of MS DOS code:-

> @ECHO OFF

> ECHO Hello, world!

> PAUSE

3. Use Notepad File menu option to Save the file as being called:  

hw01.bat

4. Go and find the file you saved: [hw01.bat]; and, left double click on it to make it run.

**NOTE**: MS DOS batch file programs are easily identifiable from other programs because it uses a picture icon of 2 cog wheels on top.  
## What are batch file programs used for?

Basically, MS DOS Batch file programs allows one to control the underlying operating system in general.

Batch file programs are created for multiple different uses...; according to the programmers own creative 'imagination'.

1. Create files/delete files

2. Create folders/delete folders

3. Read file text using the console screen...without actually having to open any other program...;  
   so, you can see program code without running it.

4. See your computer/network settings...; and, also, change these.

5. You can shut down the computer

6. If MS DOS Batch file commands are either accidentally/or else, delibrately mis-used; then, they can also create a computer 'virus'/or, 'bomb'...which causes the computer to disfunction; for example,... 

- if one were to rename/delete very important system files  
- rename drive letters  
- modify the Windows system registry   
- produce an endless loop which creates files...;  
  thus, (eventually, causing the computer to completely run out of memory)  

7. -etc.

## A list of commonly used MS DOS Commands...

**CLS** - clear the console screen  
**COPY** fileName1.txt fileName2.txt - Copies one file to become another file name/(another file is created with same contents)  
**DATE** - veiw/set date
**DEL** fileName - delete a file with the specified name  
**DEL** asterix.txt - deletes ALL [.txt] files  (deletes all text files...with the current folder directory)  
**DEL** asterix.asterix - deletes ALL files  (but, not folders...within the current folder directory)  
**DIR** - shows the current directory folder listing  
**MKDIR** folderName - Creates a new folder with the specified name  
**REN** fileName1.txt fileName2.txt - Renames a file giving it a different file name  
**RMDIR** folderName - Removes the folder with the specified name  
**TIME** - view/set time
**VER** - displays which version of MS DOS you are using 
Notepad - launches the Notepad program  
Notepad filename.ext - launches Notepad with the specified: filename + . + extension  
-etc.

**NOTE:** Above, wherever you see the word: asterix; replace this with the asterix symbol: (*), instead; unfortunately, MarkDown [.md] is NOT allowing me to include asterixes...because it uses an asterix to italicise text.

**NOTE:** Entire books have been written containing 500+ pages explaining all of the different in's and out's of the MS DOS command line system; quite obviously, I'm not going to repeat all of that same information here. Instead, I would highly recommend -assuming you wish to learn more- you either go and 'buy' a book/or, borrow one for FREE from down at your local public library; or, alternatively, do some internet research in order to go learn more(links are included, below). 

## My own personal experience with using MS DOS

Myself, I'm most definitely not an 'expert' when it comes to understanding how to use MS DOS; instead, I would honestly class myself as being a mere 'beginner'. Perhaps I know: 10/20/30 or so MS DOS commands; when, in actual fact, there are many 100's more to go and learn and know; not to mention, quite literally, 1000's of possible switches one can add in order to modify all of those commands. I must confess that I do have a really poor memory...so, that's why I write these [.md] files/github programs...just in order to help 'refesh' my memory for whenever I do, quite inevitably, tend to forget...?!

# Links

## YouTube: Video tutorials

Batch/Cmd Programming: Lesson 1 (Basics)  
- https://www.youtube.com/watch?v=kboexp3QiUg  

Batch 00 The Windows Command-Line  
- https://www.youtube.com/watch?v=JbAyxKjUPs0  

Batch Scripting - 1 - Basic Commands  
- https://www.youtube.com/watch?v=-_NleTGYE24  

Batch Programming - Learn Simply from Beginner to Advanced  
- https://www.youtube.com/watch?v=wu4Ej-SHu2Y&t=189s  

15 Command Prompt Secrets and Tricks in Windows    
- https://www.youtube.com/watch?v=7yW6Ybj6tOk  

10 Cool Command Prompt Tricks You Should Know  
- https://www.youtube.com/watch?v=TdWPEN_57mI  

Network Troubleshooting at the Command Line - CompTIA A+ 220-901 - 4.4  
- https://www.youtube.com/watch?v=-55X-koiBFg  

Introduction to Batch File Programming  
- https://www.youtube.com/watch?v=zXpCDwk3jRE  





