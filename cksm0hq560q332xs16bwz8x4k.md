---
title: "Getting Started With Conda"
seoTitle: "Getting Started with Conda Package"
seoDescription: "understand how to create Environments in your PC with Anaconda Prompt"
datePublished: Sat Aug 21 2021 16:44:30 GMT+0000 (Coordinated Universal Time)
cuid: cksm0hq560q332xs16bwz8x4k
slug: getting-started-with-conda
canonical: https://medium.com/@gouthamgosh10/getting-started-with-conda-918a9b838009
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1629564176249/OU7hyysnX.png
tags: tutorial, productivity, programming-blogs, python, machine-learning

---

We all know that Anaconda is the very popular amongst Data Scientists, python Programmers, etc. This Article helps you with getting started with Conda and setting up Anaconda in your PC. This article also helps you with Setting up Environments in your PC using Anaconda.

## What is Anaconda?

---

Wikipedia says that - Anaconda is a distribution of the Python and R programming languages for scientific computing (data science, machine learning applications, large-scale data processing, predictive analytics, etc.), that aims to simplify package management and deployment. The distribution includes data-science packages suitable for Windows, Linux, and macOS. It is developed and maintained by Anaconda, Inc., which was founded by Peter Wang and Travis Oliphant in 2012. As an Anaconda, Inc. product, it is also known as Anaconda Distribution or Anaconda Individual Edition, while other products from the company are Anaconda Team Edition and Anaconda Enterprise Edition, both of which are not free.

## Why Anaconda?

---

- Conda has very wide set of Packages for python programming which makes coding simpler compared. Anaconda packages keeps on getting updated constantly as well.
- Anaconda also comes with several IDE's and Text Editors like, Pycharm, Sypder, Jupyter notebook, etc., Leaving the user to choose on which platform does he wants to code upon.
- The UI is pretty smooth and good.
- It has a separate app called Anaconda Navigator which is really helpful to keep track of all our your installed libraries, packages and their updated versions, Conda - Installed text editors / IDE.
- It also comes with R - Studio. (you need to install it from the anaconda Navigator).
- The best part of Anaconda is it comes with Anaconda Prompt, through which we can install libraries, packages, dependencies, etc., with easy bash commands. (it might not be anything interesting for Linux/Mac OS users but when it comes to windows users, they suffer a lot with the power shell being used in the command line which is slightly different from Terminal.)

## How to Setup Anaconda in Your PC?

---

 **`Step :1`** Go to Anaconda Site - [https://www.anaconda.com/](https://www.anaconda.com/)
Visit The Anaconda website Login if you want to. Then Click on Get Started.

**`Step :2`** Download Anaconda for your PC based on Your OS
 Click on the download Anaconda Installers and select your OS.

**`Step :3`** Install Anaconda
 After the file gets downloaded, Install it. The installation Process will be pretty simple. This might take some time so have a cup of Tea and Come back.

## THE CONDA PACKAGE

Anaconda official website documentation about Conda Says that - Conda is an open-source package management system and environment management system that runs on Windows, macOS, and Linux. Conda quickly installs, runs, and updates packages and their dependencies. Conda easily creates, saves, loads, and switches between environments on your local computer. It was created for Python programs but it can package and distribute software for any language.

In its default configuration, Conda can install and manage the over 7,500 packages at [repo.anaconda.com](http://repo.anaconda.com) that are built, reviewed, and maintained by Anaconda®.

## ⚙ Setting Up the Environments in Anaconda!

---

So many people doesn't understand the purpose of creating Environments and how to create the work environment in anaconda.

## ❓**But Why to setup an environment?**

1. Setting up your own work environment is necessary because you cant keep track of every single package as there are multiple packages which keeps or suggests updating on regular basis. So some programs doesn't work if they have done in older package version and run after the package got updated. So in such case instead of avoiding of installing and reinstalling the packages you can simple create a work environment of that version of the package and run the program in that environment every time which is pretty cool and time saving.
2. Environments are highly useful especially when you are working as a team. When you are working as a team its not possible that every package that you and your friends have are of same versions. So sometimes code may not get executed properly due to the difference of the packages versions. In such cases you can clone / import your friends Environment into your PCs and work on the project without any problems.
3. The good thing about Conda is, it keeps all the history of the changes that you make so you can easily roll back if you wanted the previous version of it.

`Note: MAC/LINUX Users use the terminal and Windows users use Anaconda Prompt for the following steps:`

### (1) CREATING THE ENVIRONMENTS

1. **Creating a New Environment:**

```bash
conda create --name myenv
```

✅  When conda asks you to proceed, type `y`:

`proceed ([y]/n)?`

This creates the myenv environment in `/envs/`. No packages will be installed in this environment.

1. **Creating an Environment with Specific Version of Python:**

```bash
conda create -n myenv python=3.6
```

2. **Creating an environment with a specific package:** 

```bash
conda create -n myenv scikit-learn
```

                               (OR)

```bash
conda create -n myenv python
conda install -n myenv scikit-learn
```

3. **Creating environment with a specific version of a package:** 

```bash
conda create -n myenv scipy=0.15.0    
```

                           (OR)

```bash
conda create -n myenv python
conda install -n myenv scipy=0.15.0
```

4. **Creating environment with a specific version of Python and multiple packages:**

```bash
conda create -n myenv python=3.6 scipy=0.15.0 astroid babel
```

`myenv` - basically your environment name .

💡 **TIP:**

These are the basic ways to creating an environment. However You can do much more with `conda create` command. For details, run `conda create --help`.

### (2) **ACTIVATING THE ENVIRONMENTS**

- You can Activate the conda Environment by typing the below code:

```bash
conda activate myenv
```

`myenv` - basically your environment name 

### (3) DEACTIVATING THE ENVIRONMENTS

- You can Deactivate the conda Environment by typing the below code:

```bash
conda deactivate
```

### (4) CLONING THE ENVIRONMENTS

- You can Clone your exact conda Environment by typing the below code:

```bash
conda create --name myclone --clone myenv
```

`myclone` - basically the name of clone environment 

`myenv` - name of the environment that you want to clone 

### (5) LISTING THE ENVIRONMENTS

- basically you can view the number of existing environments that are in your PC by typing the following code:

```bash
conda env list
```

               (OR)

```bash
conda info --envs
```

### (6) SHARING THE ENVIRONMENTS

- You can share your environments with your friends or Team mates by typing the following code:

```bash
conda env export > environment.yml
```

Share the `environment.yml` file with the person whom who wanted to share.

### (7) INSTALLING THE SHARED ENVIRONMENTS

- You can Install the shared environments from your friends or Team mates by typing the following code:

```bash
conda env create -f environment.yml
```

### (8) REMOVING / DELETING THE ENVIRONMENTS

- You can remove or delete the environment by typing the following code:

```bash
conda remove --name myenv --all
```

### (9) RESTORING ENVIRONMENTS

- The good thing about Conda is, it keeps all the history of the changes that you make so you can easily roll back if you wanted the previous version of it.
- You can restore the deleted environments by using the following code:

```bash
conda list --revisions
```

Then make a note of that `REVNUM`

```bash
conda install --revision=REVNUM
```
                  (OR)

```bash
conda install --rev REVNUM
```

### (10) USING PIP COMMAND IN ENVIRONMENTS

- This is not a necessary command we don't use it all the time to install the packages or etc., but knowing about pip is definitely important.

```bash
conda install -n myenv pip
conda activate myenv
pip install streamlit
```

---

This sums up the basic things about Anaconda, Its installation and Environments. How ever you can refer to the official website of Anaconda and check its documentation if you want to dive deeply into it or to know more about it.

> 🌐 **Anaconda Official Site:**  [https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html#)

➡ There is a video about the the same in a youtube channel **Data Professor.** He explained neatly within the code editor lively. I highly recommend you to watch the video if you want to have visual explanation about the basic things about the Conda

> 🎥 **Data Professor Youtube Channel @DATA PROFESSOR:** [https://youtu.be/sDCtY9Z1bqE](https://youtu.be/sDCtY9Z1bqE)

---

## Author:

**K. SAI GOUTHAM**  

✨ [`My Git Hub`][1]  - Follow me on Git Hub and Visit My Github for Python and Data Science Related Projects.

✨ [`Medium`][2] - Follow me on medium for my articles

✨ [`My Linkedin`][3] - You can connect with me through linkedin

✨ [`Patreon`][4] - You can Follow me and Support Me by contributing to my patreon 

```bash
Thank You for visiting my article. 👋🏻
```

---
[1]:(https://www.github.com/Gouthique)
[3]:(https://www.linkedin.com/in/k-sai-goutham-828a1717b/)
[2]:(https://www.medium.com/@gouthamgosh10)
[4]:(https://www.patreon.com/Goutham)
