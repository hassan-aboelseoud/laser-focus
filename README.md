# LaserFocus
[![Channel Banner](images/Channel%20Banner.png)](https://www.youtube.com/@laserfocus314)

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/hassan-aboelseoud/laser-focus.git/HEAD)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](http://choosealicense.com/licenses/mit/)

This repository contains all the code files used in creating videos for the LaserFocus YouTube channel. A folder can be found for each playlist on the channel. Each folder contains the [Jupyter Notebooks](https://jupyter.org/) that were used to make each video in the playlist. The videos are made using the [Manim Community Edition](https://docs.manim.community/en/stable/) library for Python.


The notebooks can be run either online via [Binder](https://mybinder.org/) or offline, provided the dependencies are installed.

## Running the Notebooks Online
1. Click [here](https://mybinder.org/v2/gh/hassan-aboelseoud/laser-focus.git/HEAD) or click on "launch binder" above.
2. Select the folder corresponding to the playlist whose notebooks you want to run. Open the desired notebook and run it. You can experiment with the notebooks by running and modifying them all in your browser.

    > **Note**: Any changes you make will only be made on your local session and will be discarded once you close the page.


## Running the Notebooks Offline
The steps to run the notebooks offline are as follows:
1. Install the [Python](https://www.python.org/) programming language. The version used in this repository is [Python 3.11.4](https://www.python.org/downloads/release/python-3114/).
2. Clone this repository. You can  download and unzip this repository [here](https://github.com/hassan-aboelseoud/laser-focus/archive/refs/heads/main.zip) or by clicking Code -> Download Zip above. Alternatively, you can run the command below:

    ```sh
    git clone https://github.com/hassan-aboelseoud/laser-focus.git
    ```
3. Navigate to the cloned repository and create a Python [virtual environment](https://docs.python.org/3/tutorial/venv.html). A virtual environment is used to keep installed libraries localized to a specific project to keep them from conflicting with other projects. You can create a virtual environment by running the command below:

    ```sh
    python -m venv .venv
    ``` 
4. Activate the Python virtual environment by running the command below:
    * On Windows:

        ```sh
        .venv\Scripts\activate
        ```
    * On MacOS and Linux:

        ```sh
        source .venv/bin/activate
        ```
5. Install Jupyter Notebook by running the command below:

        ```sh
        pip install notebook
        ```
6. Install the [Manim Community Edition](https://docs.manim.community/en/stable/). The version used in this repository is v0.18.1.
    * On Windows:
        1. Install [FFmpeg](https://www.ffmpeg.org/):
            * Follow the link [here]("https://www.gyan.dev/ffmpeg/builds/") and download the file "ffmpeg-git-full.7z" under "latest git master branch build".
            * Extract the folder and rename it to "ffmpeg".
            * Move the "ffmpeg" folder to "C:\" (or any location you prefer).
            * Add "C:\ffmpeg\bin" to the PATH variable. Instructions on how to do so can be found [here](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/).
        2. Install Manim Community Edition by running the command below:

            ```sh
            python -m pip install manim==0.18.1
            ```
        3. Install a [LaTeX](https://www.latex-project.org/) distribution. LaTeX is required for rendering mathematical equations and formulae. One such LaTeX distribution is  [MiKTeX](https://miktex.org/) which can be installed here [here](https://miktex.org/download).
    * You can find the installation instructions [here](https://docs.manim.community/en/stable/installation.html) for any other operating system such as macOS or Linux.
7. Launch Jupyter Notebook by running the command below:

    ```sh
    jupyter notebook
    ```
8. Select the folder corresponding to the playlist whose notebooks you want to run. Open the desired notebook and run it. You can experiment with the notebooks by running and modifying them.