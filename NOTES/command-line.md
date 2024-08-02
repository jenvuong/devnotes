
# Command Line

## What is Command Line?
Command line interface (CLI) is the interface in which we enter commands as text inputs, which allow the computer to execute tasks.
It is the 'alternative' to Graphical user interface (GUI). This is essentially the interface or the things on the screen that we can see and click to perform tasks on the computer.

### Why not just use the GUI?
Why do we need to learn CLI if we can do the same tasks using the GUI?  
CLI can help us perform tasks more efficiently. Doing the same set of tasks through the GUI may require numerous clicks and sorting through crowds of windows.  
With CLI, a task can be executed with writing just a single line of code. With effort and habit in employing the Command Line, it will eventually become muscle-memory and improve our workflow.


## What is the Terminal?
The terminal is a text input and output environment. More simply put, it is the 'window' where we enter text inputs as commands.  

## What is a Shell?
A shell is a program that provides a user interface which handles inputs (commands) and outputs accordingly. A shell is the layer between the user and kernel. It acts as an interpreter which allows users to interact with the kernel from the command line.

### Bash
Bash (Bourne-Again SHell) is the most widely used shell program. 


## Commands
| Command | Function |
|---------|----------|
| ctrl + r | Searches through command history |
| ctrl + a | Moves cursor to start of the line |
| ctrl + e | Moves cursor to end of line* |
| ctrl + l | Clears terminal screen. Typing 'clear' does the same thing |
|**Create Files and Directories**|
| touch filename.txt | Creates file |
| echo "Content of text file" > filename.txt | Overrides content of file |
| echo "Additional content to add" >> filename.txt | Appends content to file |
| mkdir newdir | Creates a new directory/folder |
| mkdir -p newdir/seconddir | Adding p tag enables ability to create multiple directories at once |  
| **Navigate and Find Files** |
| ls | Provides an overview of where we are and a simple overview of all the files in the directory |
| ls -lah | Lists all the files in the directory. Includes additional information such as file permissions, file owner and date created. |
| cd newdir/secondir | Navigate to another directory |
| cd .. | Go back one directory. |
| cd ../.. | Go back two directories and so on |
| **Manipulating Files** |
| rm filename.txt | Deletes file |
| mv filename.txt seconddir/newfilename.txt | Renames file or moves file to new directory |
| cp filename.txt filenamecopy.txt | Makes a copy of file, set new name for copied file |

  

<sub>* NOTE: In vs code, ctrl + e is assigned to the `workbench.action.quickOpen` command.  
Solution for overriding and reassigning CTRL + E can be found [here](https://github.com/Microsoft/vscode/issues/59304)</sub>





