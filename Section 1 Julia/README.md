# Section 1 Julia
We recommend Julia 1.0+ for either of the options below because of syntax changes happened with the release of Julia 1.0. Our notebooks throughout the course only support Julia 1.0+.

## Part 1: Access to Julia and Jupyter notebook
### Option 1: Use Julia in JuliaBox
JuliaBox is an online tool to access Jupyter notebook with Julia kernels. You may create an account at <https://www.juliabox.com> to get started.

### Option 2: Download and install Julia
Alternatively, you may install Julia on your local computer if you want to do more intensive Julia programming on large datasets that JuliaBox may not be able to handle. Part of this guide comes from the guideline in <https://github.com/JuliaLang/IJulia.jl>. Upon completion, you should be able to see the Julia kernel available in Jupyter notebook:



#### Step 1: Download your (favorite) version of Julia
URL: <https://julialang.org/downloads>. We recommend the latest stable release. Follow installation instructions.

#### Step 2: Install Julia kernel into Jupyter notebook
First, enter Julia prompt:



##### Case 1: if you already have a Jupyter notebook installed

Type in the following commands, one by one, in **Julia prompt**:
```
using Pkg
Pkg.add("IJulia")
```
Then open Jupyter notebook. You will find a Julia kernel.

##### Case 2: If you don’t have Jupyter notebook on your computer

Type in the following commands in **Julia prompt**:
```
using Pkg
Pkg.add("IJulia")
using IJulia
notebook()
```
Afterwards, you may access to Jupyter notebook with Julia kernel installed at everytime by doing the following in **Julia prompt**:
```
using IJulia
notebook()
```
Or, if you had already installed Jupyter notebook from other sources (e.g., Anaconda) beforehand, you may access to the notebook by doing the following in terminal, outside **Julia prompt**:
```
jupyter notebook
```


## Part 2: Access to the Jupyter notebook for this section

The Jupyter notebook for Julia basics, [Julia syntax tutorial.ipynb](Julia_Syntax_Tutorial.ipynb), is in this folder. The way to access it depends on where you are using Julia:

### Case 1: in JuliaBox
Run the following commands in **JuliaBox’s terminal** (shown below), one line at a time:
![alt text]( "Logo Title Text 1")

```
git clone https://github.com/ORIE4741/section.git
cp -R /home/jrun/section /mnt/juliabox
```

You will then see a cloned folder named “section”. Find the folder of this Julia section, open Julia_Syntax_Tutorial.ipynb to get started!


### Case 2: in local computer
In **terminal (not Julia's prompt)**, clone the section repository by

```
git clone https://github.com/ORIE4741/section.git
```

There will be a cloned folder named "section" in your local computer. Find the folder of this Julia section, open Julia_Syntax_Tutorial.ipynb to get started!
