# Section 1 Julia

We strongly recommend using Julia 1.0+ because of major syntax changes happened with the release of Julia 1.0. Our notebooks throughout this course will only support Julia 1.0+.

You may find [some basic knowledge of UNIX commands](http://mally.stanford.edu/~sr/computing/basic-unix.html) helpful (and probably necessary). If you are using a Unix-like system like macOS, Ubuntu or Linux, you should already have a terminal available in system applications; for Windows 10, the terminal can be downloaded from [here](https://www.microsoft.com/en-us/p/windows-terminal/9n0dx20hk701?activetab=pivot:overviewtab).  

## Part 1: Access to Julia and Jupyter notebook

In this part, we show how to install Julia on your local computer. A local installation is recommended if you want to do (slightly) more intensive Julia programming on large datasets. Upon completion, you should be able to see the Julia kernel available in Jupyter notebook:

![Julia kernel](https://github.com/ORIE4741/section/blob/master/Section%201%20Julia/Julia_kernel.png "Julia kernel")

#### Step 1: Download and install Julia

Go to <https://julialang.org/downloads>. We recommend the latest stable release (v1.5.1 as of 09/08/2020). Follow installation instructions.

#### Step 2: Install Julia kernel into Jupyter notebook

If you don't have Jupyter notebook installed on your computer, we recommend installing Anaconda. It is a free and open-source distribution that includes applications like Jupyter notebook and other programming languages like Python, and should be useful even outside this course. The installer can be found at <https://www.anaconda.com/products/individual>. 

With a locally installed Jupyter notebook, we first enter the Julia prompt by opening the installed Julia application:

![Julia application](https://github.com/ORIE4741/section/blob/master/Section%201%20Julia/Julia_application.png "Julia application")

and you would be able to see the prompt as

![Julia prompt](https://github.com/ORIE4741/section/blob/master/Section%201%20Julia/Julia_prompt.png "Julia prompt")

Type in the following commands, one by one, in **Julia prompt**:

```
using Pkg
Pkg.add("IJulia")
```

Then open Jupyter notebook by typing `jupyter notebook` in command line. You will find the Julia kernel as shown at the beginning.

## Part 2: Access the Jupyter notebook for this section

The Jupyter notebook for Julia basics, [Julia syntax tutorial.ipynb](Julia_Syntax_Tutorial.ipynb), is in this folder. We will first clone this GitHub repository (if you wonder what this means, we will talk about it in roughly two weeks!) to your local computer and then run the notebook.

### Step 1: clone the GitHub repository

In **terminal (not Julia's prompt)**, clone the repository for all ORIE4741 sections by

```
git clone https://github.com/ORIE4741/section.git
```

There will be a cloned folder named "section" in your local computer at the current path.

### Step 2: Open the tutorial notebook

In terminal, again type `jupyter notebook` <sup id="a1">[1](#f1)</sup>. The terminal will start a Jupyter notebook process <sup id="a2">[2](#f2)</sup>, and you will be re-directed to the browser. Then in browser, navigate to the "section" repository you just cloned:

![Jupyter browser](https://github.com/ORIE4741/section/blob/master/Section%201%20Julia/Jupyter_browser.png "Jupyter browser")

Then open `Section 1 Julia/Julia_Syntax_Tutorial.ipynb`.

<b id="f1">1</b>: The current path determines how many files you can access to in Jupyter notebook. You may want to navigate to the root or home directory before typing this command if you want to access most of the files in your local computer. 

<b id="f2">2</b>: Don't close the terminal window or terminate the process when you use Jupyter notebook.

### References

- IJulia: <https://github.com/JuliaLang/IJulia.jl>
