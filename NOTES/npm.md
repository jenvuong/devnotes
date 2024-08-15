# NPM
Everything I have learnt so far about NPM!

NPM stands for **Node Package Manager**, and is essentially Javascript's package manager. NPM allows you to easily install packages/modules(Javascript libraries like Bootsrap or jQuery).

npmjs.com is a repository for all the NPM modules/packages. 

## Command-line 
``npm``  
Generates help page   
`npm -v`  
Checks current version  
`npm --version`   
Same as above, just long-form. This is the basic structure of long & short form flags.  
`npm init --yes`  
Generates package.json file with prefilled options.  
`npm set init-license "MIT"`  
Sets default value  
`npm get init-license`  
Checks default value  
`npm  config delete init-license`  
Deletes default value
### Install globally
`npm install -g nodemon`  
Install globally  
`npm root -g`   
Locates path where globally installed packages are installed.  
`npm remove -g nodemon`  
Uninstalls global package.



## package.json file
A file that contains all the information about your app.  
 More importantly, it lists all the app dependencies with the name and version used to create the application. This is important information when moving or transferring files, it lets you keep track of what version was used to prevent the code from breaking.   
 This is also the place where you can write NPM scripts.
 

 ## Installing Packages with Projects
 It is best practice not to include the node_modules folder when uploading to GitHub.  
 So when cloning a repository, you will need to install the relevant packages before using the code.  
 Running `npm install` will install `"dependencies"` and `"devDependencies"` listed in the package.json file.
 `npm install --production` on the other hand, will only install the packages under `"dependencies"`, leaving out the packages installed for development (`"devDependencies"`).

 ### Installing `"devDependencies"`
 The default behaviour of `npm install` installs packages under `"dependencies"`. To install packages under `"devDependencies"`, use the flag `-D`.


### Uninstalling
`npm uninstall`, `npm remove`, `npm un` and `npm rm` all do the same thing.

## Versioning
### Semantic Versioning
**v8.12.4**
The three numbers (left to right) represent the version numbers for Major, Minor and Patch versions.  
#### Patch
Minor bug fixes.
#### Minor
New features and should not break API.
#### Major
Major changes, might need to update syntax and usually breaks the API.

## Updates
Inside the package.json file, the version number for each package usually looks something like this: `"gulp": "^4.17.4"`.  
The `^` means that when you or another user runs `npm install`, Gulp will be installed to its latest Minor version.
`~` will install Gulp to its latest Patch version.
`"gulp": "*"` will install the absolute latest version of Gulp. This is usually not a good idea as it can break code and prevent code from running.