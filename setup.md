---
layout: page
title: Setup
permalink: /setup/
root: ..
---

### Obtain lesson materials

1. Create a folder called `post-docs-python` on your Desktop.
2. Download [python-novice-inflammation-data.zip][zipfile1]
        and [python-novice-inflammation-code.zip][zipfile2].
3. Save the downloaded files in the newly created `post-docs-python` folder.
4. Unzip the files.

You should now see two new folders called `data` and `code` in your `post-docs-python` directory on your
Desktop.

### Running Python

To work in Python you will need to access it from the shell using an interpreter or using a IDE like [Visual Studio Code](https://code.visualstudio.com/) or [PyCharm](https://www.jetbrains.com/pycharm/)

If you're using **macOSX**, you can run the Anaconda Navigator (installed in `/Users/<username>/anaconda3/bin` by default unless you've moved it to `Applications`) and then go to Environments -> base(root) 'Play' button -> 'Open Terminal'. This gives you a terminal that has all
the shell commands available that you've learnt already but also allows you to run python as well. Alternatively you can access the shell via the Terminal using a approach familiar to you. 

<img src="../fig/shell-anaconda.png" alt="drawing" width="40%"/>

If you're using **Windows**, you should run git-bash as you did for the shell lesson. After that, you need to enter the following commands:

```
export PATH="$PATH:/c/Users/$USERNAME/AppData/Local/Continuum/anaconda3/Scripts/:/c/Users/$USERNAME/AppData/Local/Continuum/anaconda3/"
export PATH="$PATH:/c/ProgramData/Anaconda3/Scripts/:/c/ProgramData/Anaconda3/"
```
The first line is if you installed Anaconda 3 as a user, the second is if you installed it as an admin. If you're unsure which you did, put in both! These commands make sure that Anaconda is in your path and its tools are accessible to you while you code in Python. 

### Navigate to the `post-docs-python` folder

Whether you are on macOS or Windows you should now be at a Shell prompt that is capable of running
Python. You should now navigate to your `post-docs-python` directory and view its contents to confirm the downloaded directories are there:

~~~
$ cd ~/Desktop/post-docs-python
$ ls
~~~
{: .source}

### Start a Jupyter Notebook

For this lesson we will be creating and using Jupyter Notebooks. The Jupyter Notebook is an open source web application that you can use to create and share documents that contain live code, equations, visualizations, and text. Jupyter Notebook is maintained by the people at [Project Jupyter](http://jupyter.org/). Jupyter supports over [40 programming languages](https://github.com/jupyter/jupyter/wiki/Jupyter-kernels), including Python, R, Julia, and Scala. Notebooks can be shared with others using email, Dropbox, GitHub and the [Jupyter Notebook Viewer](https://nbviewer.jupyter.org/).

### Getting started with the classic Jupyter Notebook

If you installed Anaconda on your system the Jupyter notebook is already installed on your system! Skip down to running the notebook section. If not, you can install Jupyter Notebook using `conda` or `pip`:

#### Installation with conda

~~~
$ conda install -c conda-forge notebook
~~~
{: .source}

#### Installation with pip

If you use `pip`, you can install it with : 

~~~
$ pip install notebook
~~~
{: .source}

### Running the Notebook

Congratulations, you have installed Jupyter Notebook! To run the notebook, run the following command at the Terminal (Mac/Linux) or Command Prompt (Windows):

~~~
$ jupyter notebook
~~~
{: .source}

[zipfile1]: {{ page.root }}/data/python-novice-inflammation-data.zip
[zipfile2]: {{ page.root }}/code/python-novice-inflammation-code.zip