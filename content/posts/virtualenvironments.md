+++
title = 'Virtual Environments'
date = 2023-11-30T08:40:30-05:00

+++

# 0. Summary
If you are a software developer, you need to know about virtual environments. In the first part of this post (*installation*), I go over how to install a Python virtual environment for both Macintosh and Windows. The goal is to get you going quickly. In the second part of the post (*explanation*), I provide a brief explanation about virtual environments.

# 1. Installation 

**1.1a Macintosh**

On a Macintosh, open up terminal and navigate to the directory where you want to create the virtual environment. The directory is typically where you are about to begin a new Python project. If you are in an IDE such as VS Code, open the terminal window in your project directory. To install the virtual environment type:

{{< highlight python >}}
# create a virtual environment named '.venv'
python3 -m venv .venv
{{</highlight >}}

This creates a virtual environment called .venv in a directory with the same name. To activate the virtual environment

{{< highlight python >}}
# activate the virtual environment
source .venv/bin/activate
{{</highlight >}}

**1.1b. Windows**

On Windows open the Command Prompt. Then navigate to the directory where you want to create the virtual environment.

{{< highlight python >}}
# create a virtual environment named '.venv'
python -m venv .venv
{{</highlight >}}



## 1.2 Installing Packages

Once you have installed and activated the virtual environment, you can install packages using ``pip``. For example, to install streamlit in your new virtual environment, type:

{{< highlight python >}}
# install streamlit package
pip install streamlit
{{</highlight >}}

Streamlit should now be available to you to import in your Python script.


# 2. Explanation

{{< notice question >}}
What is a virtual environment?
{{< /notice >}}

A virtual environment is an isolated environment where you can install software, Python packages (if you are using Python), and other dependencies without affecting other projects or your main environment. 

{{< notice question >}}
Why should I use a virtual environment?
{{< /notice >}}

Creating a virtual environment is important for several reasons. 

1. **Dependency Management**: Different projects may require different versions of packages. By isolating project environments, you can install different package versions without conflicts.

2. **Simplicity**: When the project is no longer needed, you can delete its virtual environment without affecting your system or other projects.

3. **Reproducibility**: By using a virtual environment, you can make the project's setup reproducible and more predictable across different machines. This is especially useful when working in a team setting.

It's also best practice to create a new virtual environment for each Python project.
