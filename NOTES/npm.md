# NPM
Everything I have learnt so far about NPM!

NPM stands for **Node Package Manager**, and is essentially Javascript's package manager. NPM allows you to easily install packages/modules(Javascript libraries like Bootsrap or jQuery).

npmjs.com is a repository for all the NPM modules/packages. 

## Command-line 
**npm**  
Generates help page   
**npm -v**  
Checks current version  
**npm --version**  
Same as above, just long-form. This is the basic structure of long & short form flags.
**npm init --yes**  
Generates package.json file with prefilled options.  
**npm set init-license "MIT"**  
Sets default value  
**npm get init-license**  
Checks default value  
**npm  config delete init-license**  
Deletes default value


## package.json file
A file that contains all the information about your app.  
 More importantly, it lists all the app dependencies with the name and version used to create the application. This is important information when moving or transferring files, it lets you keep track of what version was used to prevent the code from breaking.   
 This is also the place where you can write NPM scripts.