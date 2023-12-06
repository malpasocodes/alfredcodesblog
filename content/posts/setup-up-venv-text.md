+++
title = 'Setup a Python Virtual Environment (Text)'
date = 2023-12-03

+++

# 0. Summary
If you are a software developer, you need to know about virtual environments. In this post I go over how to setup a Python virtual environment for both Macintosh and Windows. In "Why 
setup a Virtual Environment?", I explain what is a virtual environment and why you should use it. "How to Setup a Python Virtual Environment (Video)", I provide an accompanying video.

There are four basic steps in setting up and using a Python Virtual Environment:

- Install Virtual Environment 
- Activate Virtual Environment
- Install Packages
- Deactivate Virtual Environment


# 1. Install Virtual Environment

There are many choices for installing virtual environments in Python. I recommend using ``venv``, which is a module in the standard Python library. It's battle tested and ideal for most scenarios.

On a Macintosh, open up terminal and navigate to the directory where you want to create the virtual environment. The directory is typically where you are about to begin a new Python project. (**Note**: If you are in an IDE such as VS Code, open the terminal window in your project directory.) 

To install the virtual environment type:

{{< highlight python >}}
# create a virtual environment named '.venv'
python3 -m venv .venv
{{</highlight >}}

This creates a virtual environment called .venv in a directory with the same name. 


On Windows, open the Command Prompt. Then navigate to the directory where you want to create the virtual environment.

{{< highlight python >}}
# create a virtual environment named '.venv'
python -m venv .venv
{{</highlight >}}



**2. Activate Virtual Environment**


On a Macintosh, type the following to activate the virtual environment 

{{< highlight python >}}
# activate the virtual environment
source .venv/bin/activate
{{</highlight >}}

On Windows,

{{< highlight python >}}
# activate the virtual environment
.venv\Scripts\activate
{{</highlight >}}



## 3 Install Packages

Once you have installed and activated the virtual environment, you can install packages using ``pip``. For example, to install streamlit in your new virtual environment, type:

{{< highlight python >}}
# install streamlit package
pip install streamlit
{{</highlight >}}

Streamlit should now be available to you to import in your Python script.


