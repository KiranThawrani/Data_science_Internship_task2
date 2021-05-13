# Data_science_Internship_task2
Data_science_Internship_task2

## Flask web Development Application:

The first venv in the command is the name of the Python virtual environment package, and the second is the virtual environment name that I'm going to use for this particular environment.
With this command, I'm asking Python to run the venv package, which creates a virtual environment named venv.
In Flask, handlers for the application routes are written as Python functions, called view functions.
To complete the application, you need to have a Python script at the top-level that defines the Flask application instance.
When you activate a virtual environment, the configuration of your terminal session is modified so that the Python interpreter stored inside it is the one that is invoked when you type python.
Installing a package from PyPI is very simple, because Python comes with a tool called pip that does this work (in Python 2.7 pip does not come bundled with Python and needs to be installed separately).
For those versions of Python, you need to download and install a third-party tool called virtualenv before you can create virtual environments.
When you install packages in a virtual environment, the system-wide Python interpreter is not affected, only the copy is.
The next step is to install Flask, but before I go into that I want to tell you about the best practices associated with installing Python packages.
Imagine a situation where you have completed a web application using version 0.11 of Flask, which was the most current version of Flask when you started, but now has been superseeded by version 0.12. You now want to start a second application, for which you'd like to use the 0.12 version, but if you replace the 0.11 version that you have installed you risk breaking your older application.
The __name__ variable passed to the Flask class is a Python predefined variable, which is set to the name of the module in which it is used.
In Python, packages such as Flask are available in a public repository, from where anybody can download them and install them.
To address the issue of maintaining different versions of packages for different applications, Python uses the concept of virtual environments.
The script above simply creates the application object as an instance of class Flask imported from the flask package.
If your Python interpreter was installed globally for all the users of your computer, chances are your regular user account is not going to have permission to make modifications to it, so the only way to make the command above work is to run it from an administrator account.
So the solution to have complete freedom to install any versions of your packages for each application is to use a different virtual environment for each application.
A virtual environment is a complete copy of the Python interpreter.
If you are using any version of Python older than 3.4 (and that includes the 2.7 release), virtual environments are not supported natively.
Welcome! You are about to start on a journey to learn how to create web applications with Python and the Flask framework.
The official Python package repository is called PyPI, which stands for Python Package Index (some people also refer to this repository as the "cheese shop").
The Flask application instance is called app and is a member of the app package.
If your operating system does not provide you with a Python package, you can download an installer from the Python official website.
The pip tool is going to download the package from PyPI, and then add it to your Python installation.
To make sure your Python installation is functional, you can open a terminal window and type python3, or if that does not work, just python.
Since this application is running in a development environment, Flask uses the freely available port 5000.
The app variable is defined as an instance of class Flask in the __init__.py script, which makes it a member of the app package.
Starting with version 1.0, Flask allows you to register environment variables that you want to be automatically imported when you run the flask command.
If you are using Microsoft Windows along with WSL or Cygwin, note that you will not be using the Windows native version of Python, but a Unix-friendly version that you need to obtain from Ubuntu (if you are using WSL) or from Cygwin.
Once you become more familiar with Flask and the example application you can access the code directly from GitHub if the typing becomes too tedious.
From that point on, every Python script that you have on your system will have access to this package.
If you find this confusing, you can replace the second venv with a different name that you want to assign to your virtual environment.
In Python, a sub-directory that includes a __init__.py file is considered a package, and can be imported.
In general I create my virtual environments with the name venv in the project directory, so whenever I cd into a project I find its corresponding virtual environment.
Posted by Miguel Grinberg under Flask, Programming, Python.
After the command completes, you are going to have a directory named venv where the virtual environment files are stored.
If you go to the Flask website, you are welcomed with a very simple example application that has just five lines of code.
You are going to see that the routes module needs to import the app variable defined in this script, so putting one of the reciprocal imports at the bottom avoids the error that results from the mutual references between these two files.
$ python3 Python 3.5.2 (default, Nov 17 2016, 17:05:23) [GCC 5.4.0 20160609] on linux Type &quot;help&quot;, &quot;copyright&quot;, &quot;credits&quot; or &quot;license&quot; for more information.
Flask uses the location of the module passed here as a starting point when it needs to load associated resources such as template files, which I will cover in Chapter 2.
Do you see the problem? It would be ideal if it was possible to install Flask 0.11 to be used by your old application, and also install Flask 0.12 for your new one.
The two strange @app.route lines above the function are decorators, a unique feature of the Python language.
Note that in some operating systems you may need to use python instead of python3 in the command above.
If you work with multiple terminal windows open at the same time, it is perfectly fine to have different virtual environments activated on each one.
This means that when a web browser requests either of these two URLs, Flask is going to invoke this function and pass the return value of it back to the browser as a response.
The Python interpreter is now waiting at an interactive prompt, where you can enter Python statements.
Also, the terminal prompt is modified to include the name of the activated virtual environment.
In this first chapter, you are going to learn how to set up a Flask project.
If you don't have Python installed on your computer, go ahead and install it now.
On the Linux and Mac OS X versions of Python you can also exit the interpreter by pressing Ctrl-D.
View functions are mapped to one or more route URLs so that Flask knows what logic to execute when a client requests a given URL.
Let's create a package called app, that will host the application.
The app package is defined by the app directory and the __init__.py script, and is referenced in the from app import routes statement.
Since environment variables aren't remembered across terminal sessions, you may find tedious to always have to set the FLASK_APP environment variable when you open a new terminal window.
Both routes are associated with the only view function in the application, so they produce the same output, which is the string that the function returns.
The Zip link is a download link for a zip file including the entire application up to and including the changes in the chapter.
The bottom import is a workaround to circular imports, a common problem with Flask applications.
But for now, you have confirmed that Python is installed on your system.
The Browse link will open the GitHub repository for Microblog at the place where the changes for the chapter you are reading were added, without including any changes introduced in future chapters.
So what goes in the routes module? The routes are the different URLs that the application implements.
Some installations use python for Python 2.x releases and python3 for the 3.x releases, while others map python to the 3.x releases.
Note 2: If you would like to support my work on this blog, or just don't have patience to wait for weekly articles, I am offering the complete version of this tutorial packaged as an ebook or a set of videos.
If this statement does not give you any errors you can congratulate yourself, as Flask is installed and ready to be used.
The application will exist in a package.
For all practical purposes, passing __name__ is almost always going to configure Flask in the correct way.
The application then imports the routes module, which doesn't exist yet.
Regardless of the method you used to create it, you should have your virtual environment created.
The output from flask run indicates that the server is running on IP address 127.0.0.1, which is always the address of your own computer.
The from app import app statement imports the app variable that is a member of the app package.
Do you see the application route mappings in action? The first URL maps to /, while the second maps to /index.
Virtual environments have the added benefit that they are owned by the user who creates them, so they do not require an administrator account.
At the beginning of each chapter, I'm going to give you three GitHub links that can be useful while you work through the chapter.
If you find this confusing, you can rename either the package or the variable to something else.
If this does not make complete sense yet, it will in a little bit when you run this application.
If you enter any other URL you will get an error, since only these two URLs are recognized by the application.
When you import a package, the __init__.py executes and defines what symbols the package exposes to the outside world.
If you would you like to support my MicroPython tutorial series on this blog and as a reward have access to the complete tutorial nicely structured as an ebook and 6+ hours of video material, you can now order it from my Courses site.
The Diff link will open a graphical view of all the changes that were made in the chapter you are about to read.
But even without that complication, consider what happens when you install a package as above.
If you prefer to set the environment variable manually, that is perfectly fine, as long as you always remember to do it.
Downloading the code from GitHub can save you a lot of typing, but I strongly recommend that you type the code yourself, at least for the first few chapters.
Another peculiarity is that the routes module is imported at the bottom and not at the top of the script as it is always done.
Instead of repeating that trivial example, I'm going to show you a slightly more elaborate one that will give you a good base structure for writing larger applications.
Applications deployed on production web servers typically listen on port 443, or sometimes 80 if they do not implement encryption, but access to these ports require administration rights.
All the code examples presented in this tutorial are hosted on a GitHub repository.
In this case, the @app.route decorator creates an association between the URL given as an argument and the function.
The changes made to your terminal session are all temporary and private to that session, so they will not persist when you close the terminal window.
To exit the interactive prompt, you can type exit() and press Enter.
This view function is actually pretty simple, it just returns a greeting as a string.
If you are using Microsoft Windows, use set instead of export in the command above.
Interestingly, this method of installing packages will not work in most cases.
This address is so common that is also has a simpler name that you may have seen before: localhost.
Before I end this chapter, I want to mention one more thing.
A common pattern with decorators is to use them to register functions as callbacks for certain events.
You can also find me on Facebook, Google+, LinkedIn, Github and Twitter.
On Windows, the exit shortcut is Ctrl-Z followed by Enter.
