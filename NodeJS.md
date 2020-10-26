Monday, 26. October 2020

# NodeJS lessons

## installing nodejs

Download from
[node-v15.0.1-linux-x64.tar.xz](https://nodejs.org/dist/v15.0.1/node-v15.0.1-linux-x64.tar.xz)

extract to opt/node

setting up environment variables. Open console and:

	gedit ~/.profile


in the profile file add following lines :

	PATH="$PATH:/opt/node/node-v15.0.1-linux-x64/bin"
	export PATH
	
and **save**

	source ~/.profile
	node --version 
should now show:

	v15.0.1
<br><br>

## npm commands

open a terminal in the working folder,
this command shows the nodes in the folder and type *npm ls*. if a valid package.json exists it should show.
eg:

	> npm ls
	hello-npm@1.0.0 /home/sathimantha/DEP/npm-demos/hello-npm
	├── bootstrap@4.5.3
	└── jquery@3.5.1


## node-js packages
A valid node package should contain *package.json* file with following format:

	{
	    "name": "hello-npm",
	    "version": "1.0.0",
	    "dependencies": {
	        "bootstrap": "^4.5.3",
	        "jquery": "^3.5.1"
	    }
	}
	
[npmjs.com](https://www.npmjs.com/) has a collection of publicly available packages. Install packages using:

	npm i <package name>
<br>

