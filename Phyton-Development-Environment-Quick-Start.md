# Python Development Environment Quick Start

* [About this hands-on](#about)
* [Anaconda](#AnacondaChapter)
    * [Conda](#conda)
    * [Managing Packages](#managing)
    * [Environments](#environments)

    * [Download and installing Anaconda](#anaconda)
    * [New iPython notebook](#notebook)

<a name="about"/>
Until now we discover how to write our first program in Python and how to install the required environment.  Alternately, we can download and install an environment that can simplify package management and deployment (which comes with pre-installed libraries). 
This hand-on is intended to be a "Simple Beginner’s guide" that provides a fast-paced introduction to the Python Development Environment  [Anaconda](https://www.continuum.io/why-anaconda).

<a name="AnacondaChapter"/>
## Anaconda
 
I would recommend use [Anaconda](https://www.continuum.io/why-anaconda) available for Windows, OS X or Linux, 32- or 64-bit. Anaconda is a freemium open source distribution of the Python and R programming languages for large-scale data processing, predictive analytics, and scientific computing.

Why Anaconda? Anaconda is a distribution of packages built for data science. It comes with conda, a package and environment manager. In a real project You will be using conda to create environments for isolating your projects that use different versions of Python and different packages. You could also use it to install, uninstall, and update packages in your environments. 

With Anaconda, it's simple to install the packages you will often use in real data science work. You'll also use it to create virtual environments that make working on multiple projects much less mind-twisting. Anaconda solved a lot of issues related with packages and multiple Python versions. 

<a name="Conda"/>
### Conda
Anaconda is actually a distribution of software that comes with `conda`, `Python`, and many scientific packages and their dependencies. The application conda is a package and environment manager. Anaconda is a fairly large download (~500 MB) because it comes with the most common data science packages in Python. There is also **Miniconda**, a smaller distribution that includes only conda and Python. You can still install any of the available packages with conda, it just doesn't come with them. Using conda to manage your packages and environments will reduce future issues dealing with the various libraries you'll be using. 

<a name="managing"/>
### Managing Packages
Package managers are used to install libraries and other software on your computer. You are already familiar with `pip`, it’s the default package manager for Python libraries. `Conda` is similar to `pip` except that the available packages are focused around data science while `pip` is for general use. `conda` is not Python specific and can also install non-Python packages. However, not all Python libraries are available from the Anaconda and conda and for this reason you can still use `pip` alongside `conda` to install packages.

<a name="environments"/>
### Environments
Along with managing packages, Conda is also a virtual environment manager. It's similar to [`virtualenv`](http://docs.python-guide.org/en/latest/dev/virtualenvs/). **Environments allow you to separate and isolate the packages you are using for different projects**. Sometimes you could be working with code that depends on different versions of some library. For example, you could have code that uses new features of a package, or code that uses old features that have been removed from the package. It’s practically impossible to have two versions of the same package installed at once. Instead, you should make an environment for each version of the package then work in the appropriate environment for the project.  This issue happens a lot when dealing with Python 2 and Python 3 at the same time.

We can also export the list of packages in an environment to a file, then include that file with your code. This allows other people to easily load all the dependencies for our code. Pip has similar functionality with `pip freeze > requirements.txt` (“freeze” the current state of the environment packages).


-----  -----
I personally prefer iPython Notebooks from Anaconda because it provides a lot of good features for documenting while writing the code itself and you can choose to run the code in blocks rather than the line by line execution in the terminal environment. We will use iPython environment for this complete hands-on tutorial. I can say that using Anaconda has made my life working with data much more pleasant.

<a name="anaconda"/>
### Download and installing Anaconda
Visit the [Anaconda](https://www.continuum.io/downloads) web page and download the correct version of package acording your OS system and follow the instructions. 

After your installation proces is finished you can start iPython notebook by writing `ipython notebook` on your terminal:
``` 
torres@vm:~$ jupyter notebook

```


This will launch a new browser window (or a new tab) showing the Notebook Dashboard on a localhost to the URL of your Notebooks, by default http://127.0.0.1:8888. Windows users need to open up their Command Prompt. You'll see a dashboard with all your Notebooks. You can launch your Notebooks from this control panel that allows (among other things) to select which notebook to open or create a new one. 

<a name="notebook"/>
### iPython notebooks
You can create a new iPython notebook by simply clicking on the **new** button  in the top. The interface shows **In\[\*\]**  for inputs and **Out\[\*\]** for output. You can execute a code by pressing *“Shift + Enter”* or *“ALT + Enter”*, if you want to insert an additional row after.  Copy \& paste the previous code example `GuessNumber.py` at **In\[1\]**, press “Shift + Enter” and introduce your guess number.

![ipythonnotebookExample](https://github.com/jorditorresBCN/Python-Quick-Start/blob/master/img/ipythonnotebookExample.png)

