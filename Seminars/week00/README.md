# Week description

This week's content focuses on various support materials from programming, data analytics, and machine learning fields. Feel free to refer back to this list during the course.

### Contents

* Main tools to operate with during this course
* Supplementary materials for different topics
* Instructions for setting up local envinroments

---

# Main tools to operate with during this course

* [Colab](https://colab.research.google.com/#scrollTo=-Rh3-Vt9Nev9)  - check the main page for some useful links (just click "cancel" in the beginning).
* [Google](https://www.google.com/) & [StackOverflow](https://stackoverflow.com/) - you know what to do! But don't blindly copy answers, **retype** the code and **understand** what's going on.
* [NumPy](https://numpy.org/doc/stable/user/) - *quickstart* & *basics* is a must, *array creation* and *indexing* topics in fundamentals are also important.
* [Pandas](https://pandas.pydata.org/docs/user_guide/) - a complete description of pandas features. Just search for a relevant topic when you get stuck.
* [Matplotlib](https://matplotlib.org/stable/tutorials/index.html) & [Plotly](https://plotly.com/python/) - key graphics libraries. In most cases, a basic tutorial + stackoverflow/google answers will suffice.
* [Seaborn](https://seaborn.pydata.org/tutorial/introduction.html) - it is built on the roof of Matplotlib and is considered as a superset of the Matplotlib library.
* [Scikit-learn](https://scikit-learn.org/stable/user_guide.html) - great for educational/research purposes. Check out the user guide for tutorials on many ML aspects.
* [Pytorch](https://pytorch.org/tutorials/beginner/basics/intro.html) - one of the main tools for working with neural networks

---

# Supplementary materials

[Scientific Python](https://lectures.scientific-python.org/index.html) is a set of tutorials on the scientific Python ecosystem: a quick introduction to central tools and techniques, all in one place. 

**PYTHON**

- If you're a zero-level programmer, the best way to start is to look through some sort of coherent tutorial that covers all the main aspects of Python programming.
- For example, [Stepik](https://stepik.org) has a number of courses on Python and other Data science tools.
- [Программирование на Python](https://stepik.org/course/67/info) from `Bioinformatics Institute' is a good place to start.
- [Класс Python от Google](https://developers.google.com/edu/python?hl=ru) can be a good way to start as well.
- If you know the basics, but would like to sharpen your skills, then you can solve tasks on [LeetCode](https://leetcode.com/), [Yandex CodeRun](https://coderun.yandex.ru/) or any other similar platform.


**NUMPY**
- [Lecture on Numpy from Robert Johansson](https://nbviewer.org/github/jrjohansson/scientific-python-lectures/blob/master/Lecture-2-Numpy.ipynb) - implented as IPython notebook with many examples
- [Numpy tutorial by Stanford CS231](https://cs231n.github.io/python-numpy-tutorial/)
- [A set of tasks for you to practice](https://github.com/rougier/numpy-100)

**PANDAS**
- [Community Tutorials](https://pandas.pydata.org/docs/getting_started/tutorials.html)
- [Pandas CheatSheet](https://pandas.pydata.org/Pandas_Cheat_Sheet.pdf), but you may also find alternatives cheat sheets if this one does not serve you
- [Практикум по Pandas](https://stepik.org/course/111629/info) on Stepik, can serve as a task book

**MATPLOTLIB**

- [Official tutorials](https://matplotlib.org/stable/tutorials/index.html)
- [Some tutorial on Kaggle](https://www.kaggle.com/code/prashant111/matplotlib-tutorial-for-beginners) 

**STATISTICS**

- [Основы статистики](https://stepik.org/course/76/info) - beginner friendly
- С. Гланц. Медико-биологическая статистика. Пер. с англ. — М., Практика, 1998. — 459 с

**MACHINE LEARNING**

- [Машинное обучение 1 (ПМИ ФКН)](https://github.com/esokolov/ml-course-hse/tree/master)
- [Хэндбук Яндекса по машинному обучению](https://education.yandex.ru/handbook/ml)
- [Курс лекций К.В.Воронцова](http://www.machinelearning.ru/wiki/index.php?title=%D0%9C%D0%B0%D1%88%D0%B8%D0%BD%D0%BD%D0%BE%D0%B5_%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D0%B5_%28%D0%BA%D1%83%D1%80%D1%81_%D0%BB%D0%B5%D0%BA%D1%86%D0%B8%D0%B9%2C_%D0%9A.%D0%92.%D0%92%D0%BE%D1%80%D0%BE%D0%BD%D1%86%D0%BE%D0%B2%29)
- [Stanford CS229: Machine Learning](https://cs229.stanford.edu/)

---

# Instructions for setting up local envinroment

If you are not a fan of reinstalling all packages everytime you launch Colab, it is recommended to set up a consistent local Python Environment and work in Jupyter Notebook. This will also be useful during your other courses on our master's programme, and generally this is something you are expected to know as a Data Science specialist (bioinformatics or not).

There are several things to consider:
1. Follow either [this tutorial](https://docs.jupyter.org/en/latest/install/notebook-classic.html) or instructions below.
2. First of all, understand what your OS is capable of. Unix-like OS (MacOS, Linux) come with Unix shell. If you're a Windows user, consider installing WSL 2 (Windows Subsystem for Linux), this will help you greatly when working with bioinformatics tools locally, and you will learn bash!
3. We recommend installing Anaconda distribution for installing Python and Jupyter. There are several installers available now, such as Anaconda and Miniconda. The difference is described [here](https://stackoverflow.com/questions/45421163/anaconda-vs-miniconda). I would recommend installing Miniconda since right now you don't need so many pre-installed packages. The process is described below, but also check the [original instruction](https://conda.io/projects/conda/en/latest/user-guide/install/index.html) in case you need any alternatives.
4. If you chose Miniconda, visit [this page](https://docs.anaconda.com/miniconda/#quick-command-line-install) and follow instructions for installation. At the end of the page, the quick command line install is listed. For example, for Linux (also works for WSL 2):
```
mkdir -p ~/miniconda3
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh -O ~/miniconda3/miniconda.sh
bash ~/miniconda3/miniconda.sh -b -u -p ~/miniconda3
rm ~/miniconda3/miniconda.sh
~/miniconda3/bin/conda init bash
```
5. After installation, create and activate conda environment and install Jupyter.
```
conda create -n ml_bioinf  # creates new virtual env (ml_bioinf is the name of it, you can change this)
conda activate ml_bioinf   # activate environment in terminal
conda install jupyter      # install jupyter notebook
jupyter notebook           # launch jupyter notebook
```
6. You're good to go! But you may also consider installing a Python IDE that suits you. Skip that step in case you're planning only to work in Jupyter Notebook, since it can open in browser window.\
Popular choices: 
    1. VS Code
    2. PyCharm
    3. Spyder
Depending on your choice and the OS you're working with, the installation process may vary.
