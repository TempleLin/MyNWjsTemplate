How it's configured: (Everything is installed and set in this template. Just type "npm install" in terminal to start.)
    "npm init -y" in terminal.
    "npm install nw@[your wanted version]-sdk nw-builder -D" in terminal.
    
    Set "scripts" attributes accordingly under package.json.
        ex:
            "dev": "nw src/",
            "prod": "nwbuild --platforms win32,win64,osx64,linux32,linux64 --buildDir dist/ src/"

    Create src folder.
    Create app, assets, styles, views folder under src folder.
    "cd src" on terminal.
    "npm init -y" on terminal.
    Set "main" and "window" attributes accordingly under src/package.json.


To run in development mode, "npm run dev" in terminal.
To build, "npm run prod" in terminal.

Tutorial resource used: https://www.youtube.com/watch?v=5UsGnjPYxLU

Note: 
1.Path of the directory won't be near the executable when distributed.
	To get current executable's directory: path.dirname(process.execPath);
2.Might need administration when opening CMD for distribution.