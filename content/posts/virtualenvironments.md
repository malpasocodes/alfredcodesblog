+++
title = 'Virtual Environments'
date = 2023-11-30T08:40:30-05:00

+++

# Summary
If you are a software developer, you need to know about virtual environments. In the first part of this post (installation), I go over how to install a virtual environment for Python in both a Mac and Windows environemnt. The goal is to get you going quickly. In the second part of the post (explanation), I provide a brief explanation about virtual environments.

# Installation 

On a macintosh, open up terminal and navigate to the directory where you want to create the virtual environment. The directory is typically where you are about to begin a new Python project. To install the virtual environment type:

{{< highlight python >}}
# create a virtual environment named '.venv'
python3 -m venv .venv
{{</highlight >}}

This creates a virtual environment called .venv in a directory with the same name. To activate the virtual environment

{{< highlight python >}}
# activate the virtual environment
source .venv/bin/activate
{{</highlight >}}

On Windows open the Command Prompt. Then navigate to the directory where you want to create the virtual environment.

{{< highlight python >}}
# create a virtual environment named '.venv'
python -m venv .venv
{{</highlight >}}

{{< highlight python >}}
# activate the virtual environment
.venv\Scripts\activate
{{</highlight >}}

# Explanation



{{< notice question >}}
What is a virtual environment?
{{< /notice >}}

A virtual environment is an isolated environment where you can install software, Python packages (if you are using Python), and other dependencies without affecting other projects or your main environment. 

{{< notice question >}}
Why should I use a virtual environment?
{{< /notice >}}

Creating a virtual environment is important for several reasons. 

GitHub Copilot: A virtual environment is an isolated environment where you can install software and Python packages without affecting your system's other Python projects. It's essentially a folder/directory that contains a Python installation (of a particular version), plus a few additional tools.

Creating a virtual environment is important for several reasons:

1. **Dependency Management**: Different projects may require different versions of packages. By isolating project environments, you can install different package versions without conflicts.

2. **Simplicity**: When the project is no longer needed, you can delete its virtual environment without affecting your system or other projects.

3. **Reproducibility**: By using a virtual environment, you can make the project's setup reproducible and more predictable across different machines. This is especially useful when working in a team setting.

It's also plain best practice to create a new virtual environment for each Python project.

{{< notice question >}}
How do I create a virtual environment in Python?
{{< /notice >}}

There are several ways to create virtual environments in Python. For most projects, I recommend I going with ``venv`` which comes packaged with your Python installation. 

On a Macintosh, 

- Open Terminal
- Navigate to the directory where you want to create the virtual environment


# Create a virtual environment named '.venv'
python3 -m venv venv

# Activate the virtual environment
source venv/bin/activate
