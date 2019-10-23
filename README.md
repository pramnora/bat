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

## How to create a batch file program/and, then, make it execute...

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

7. Programming, using loops/variables/if statements/GOTO/labels/-etc.

8. -etc.

## MS DOS PROGRAMMING

Most MS DOS commands are very simple...such as DIR...which lists what is the current directory folders/files;  
however, the simple execution of 'one' command is NOT really a 'programming construct'.

MS DOS does include some programming related concepts/contructs, namely,...

**VARIABLE NAMES**

> SET myName="xyz"  

> ECHO %myName%

**NOTE:** There must be no space between var="value"; otherwise, the ECHO var command will not work!

**GOTO** statements/plus, label names...  

> start:    

> ECHO This is a GOTO form of 'endless loop...'  

> GOTO start

**NOTE:** In order to break out of a running 'endless loop'...;   
then, do combination keypress: [CTRL] + [C] to cancel...;        
a prompt will appear asking if you really wish to cancel the batch job, Y/N?    
Type: Y;   
then, press [ENTER] key to stop. 

**FOR** LOOPS...  

> FOR %%n IN (1,2,3) DO ECHO %%n

**NOTE:** The above code is how you would write a FOR loop being included inside of a DOS BATCH program file: [.bat];   
in order to get the same FOR loop code to work at the command prompt...you would write it as follows:  

> FOR %n IN (1,2,3) DO ECHO %n

**MODULES** 

Modularity, is where one MS DOS batch file program can easily be made to call a next.

So, for example...if we had 2 x separate MS DOS program files: [a.bat]/[b.bat];     
...and, we wished to link both of these files to run together;       
to, automatically, run/execute one after the other...we would write it as...  

Filename 1: a.bat

> @ECHO OFF  

> CLS  

> ECHO This is file [a.bat]  

> PAUSE  

> b.bat  

Filename 2: b.bat

> @ECHO OFF  

> CLS  

> ECHO This is file [b.bat]  

> PAUSE  

**NOTE** You simply call the named batch file program at the end of the file: [b.bat]...;   
         in order to link both: [a.bat]/[b.bat].

Too, there are IF statements.../-etc.

## A list of commonly used MS DOS Commands...

### File management related commands

**COPY** fileName1.txt fileName2.txt - Copies one file to become another file name/(another file is created with same contents)  
**DEL** fileName - delete a file with the specified name  
**DEL** asterix.txt - deletes ALL [.txt] files  (deletes all text files...with the current folder directory)  
**DEL** asterix.asterix - deletes ALL files  (but, not folders...within the current folder directory)  
**DIR** - shows the current directory folder listing  
**MKDIR** folderName - Creates a new folder with the specified name  
**REN** fileName1.txt fileName2.txt - Renames a file giving it a different file name  
**RMDIR** folderName - Removes the folder with the specified name  
**TREE** outputs the current folder/file directory in tree branch format to the console output screen  

**NOTE:** Above, wherever you see the word: asterix; replace this with the asterix symbol: (*), instead; unfortunately, MarkDown [.md] is NOT allowing me to include asterixes...because it uses an asterix to italicise text.

**NOTE:** MS DOS Commands are NOT 'case sensitive'...so, DIR/Dir/dir...are all regarded as being entirely equivalent.        

### Launch program files related commands

**CALC** - launches the calculator program    
**Notepad** - launches the Notepad program  
**Notepad** filename.ext - launches Notepad with the specified: filename + . + extension    
**MSPaint** - launches MS Paint program for doing drawing/painting  
**WRITE** - launches a more sophistcated word processor than is the simple Notepad...;  
            (you can add colours/pictures/other formatting/-etc.)  

### Networking related commands

**IPCONFIG** - shows the computer system info. such as IP address    
**NETSTAT** - Lists running processes  
**PING** URL - tests internet connection between two computers  
**WMIC** logicaldisk get name - shows all available Drive letters   

### Pipe related commands

dir | clip - sends to the clipboard the current directory listing of all files/folders;    
             (next, one can open Notepad to copy and paste from the clipboard)  
notepad (used in conjunction with the above; when notepad opens...just do a [CTRL] + [V] to paste.  

dir > showdir.txt - sends to the file: [showdir.txt] the current directory listing of all files/folders  




### System related commands

**DATE** - view/set date  
**REGEDIT** - allows one to view/change Windows System Registry entries  
**SHUTDOWN** - shuts the computer system down  
**TIME** - view/set time  
**VER** - displays which version of MS DOS you are using   

### Text related commands

**COLOR** - allows the user to change the console screen: background/foregroud colours using hex codes: 0-F.   
**CLS** - clear the console screen  
**ECHO** text - ECHO's to the console screen whatever text is being written after the ECHO command statement  
**ECHO.** - The ECHO commands statement preceeded with a dot: (.)...means output a vertical blank line inside of the console screen  
**PROMPT** text - allows one to change the MS DOS Window command prompt text  
**TITLE** text - allows one to change/replace the MS DOS Prompt window title text  
**TYPE** filename.ext - outputs the file text onto the console screen; (without actually executing the commands if a program file)  

-etc.

**NOTE:** Entire books have been written containing 500+ pages explaining all of the different in's and out's of the MS DOS command line system; quite obviously, I'm not going to repeat all of that same information here. Instead, I would highly recommend -assuming you wish to learn more- you either go and 'buy' a book/or, borrow one for FREE from down at your local public library; or, alternatively, do some internet research in order to go learn more(links are included, below). 

**NOTE:** It's possible to have 'multiple' Command Prompt windows open together, all at once; therefore, you are not confined to using just one single Command Prompt window, alone.

## Some further tips on using the Command Prompt line

Here are some further useful tips when you are working at the MS DOS Command Prompt line...

1 - You can use TAB to help auto-complete commands you are trying to type in...

So, if there is a file called: xray.txt...inside of the current directory folder...;  
you don't need to type in full file name + file name extension...;  
but, instead, simply type in the first letter of the filename:  

C:\> x (then, press [TAB] key...which will  auto-fill in the rest...
C:\> xray.txt

**NOTE:** If there exists more than one file starting with the letter 'x';  
then, just keep on repeatedly pressing [TAB] to get to the next file beginning with letter 'x'; and, so on... 

2 - If you wish to see a list of commands you've typed in before;   
    then, use the UP ARROW key to take you backwards through the command history list;  
    pressing the DOWN ARROW key moves you forwards through the command history list.   

3 - In order to move your cursor to the beginning/or, end of the line use...  
    a - press [Home] takes you to the beginning of the line  
    b - press [End] takes you to the end of the line  

4 - [CTRL] + [LEFT ARROW]/or, [RIGHT ARROW] moves the cursor 1 word at a time...going either backwards/forwards. 

5 - Pressing function key: [F7], will give you full command history listing...showing all the commands you had typed in before.  

## My own personal experience with using MS DOS

Myself, I'm most definitely not an 'expert' when it comes to understanding how to use MS DOS; instead, I would honestly class myself as being a mere 'beginner'. 

Perhaps I know: 30 or so MS DOS commands(half of which I can actually at any one time recall); when, in actual fact, there are many 100's more to go and learn and know; not to mention, quite literally, 1000's of possible switches one can add in order to modify all of those commands.

I must confess that I do have a really poor memory...so, that's why I write these [.md] files/github programs...just in order to help 'refesh' my memory for whenever I do, quite inevitably, tend to forget...?!

## CONCLUSION

MS DOS, represents a whole entire operating system in itself; and, therefore, the list of commands/plus, all possible switches used to modify those commands is 'huge'...!

Any programmer/or, like me, potential programmer...who can understand how to use MS DOS commands really well...will be able to program and manipulate a Windows based computer machine system any how they please. 

So, what I'm saying here is, quite simply, this...if you are a programmer; then, it's also necessary to know MS DOS commands.

## WINDOWS POWERSHELL

Windows has already brought out a different command line window which is used to replace the MS DOS Command Prompt; and, it is called: Powershell. 

Powershell, is a much more complex program -in my own view- which also contains loads and loads of different commands/plus, reportedly, commands related to the programming side of things is far better.  

1. **Open Windows Powershell within Windows Command Prompt window**

In order to run Powershell -(which, normally, has a 'blue' background screen when you run the program independently/however, if you run it directly from within MS DOS, then, the background remains coloured in 'black')- just type in after the DOS Command Prompt...

C:\> Powershell

...and, the MS DOS Prompt changes over to become as follows:  

PS C:\>

**NOTE:** DOS command usage will also work inside of the Powershell window.

2. **Open Windows Powershell as being an entirely separate window**

An alternate way to open up the Powershell program window is...

Do a combination keypress: [WINDOWS PICTURE ICON KEY] + [R]...opens up the Run dialog box...then, type in: Powershell...and, press the [OK] button...and, a window should now open up showing the 'blue' Powershell screen...ready for typing commands into.

**NOTE:** Powershell, uses both DOS commands such as DIR to obtain a current folder/files DIRrectory listing.../and, UNIX style commands such as: LS...which also achieves doing exactly the same thing.

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





