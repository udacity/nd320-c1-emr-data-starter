
If you want to download course exercises to your local computer, instead of using the provided workspaces, you will find the information below helpful.

### Lesson Folder

This repo contains a folder for each `lesson` and one `project` folder.

Example
```
lesson-1-hello
lesson-2-world
lesson-3-foo
lesson-4-bar
project
```

Each `lesson` folder is named using the naming convention of `lesson-#-name-of-lesson`.

Example
```
lesson-1-hello
```


### Exercises Folder

Each `lesson` folder contains an `exercises` folder. This `exercises` folder should contain all files and instructions necessary for the exercises along with the solution. The solutions for these exercises will be shared with students. See the `README` in the `exercises` folder for information about folder structure.

### Project Folder

The `project` folder should contain all files and instructions necessary for setup. If possible, a set of instructions should be provided for both Udacity workspaces and a way to work locally (for both MacOS and Windows OS). At a minimum, one set of instructions should be provided. A `README` template has been provided in the project folder. This template layout should be used to write your README.

## Getting Started

Instructions for how to get a copy of the project running on your local machine.

### Dependencies
Using Anaconda consists of the following:

1. Install [`miniconda`](http://conda.pydata.org/miniconda.html) on your computer, by selecting the latest Python version for your operating system. If you already have `conda` or `miniconda` installed, you should be able to skip this step and move on to step 2.
2. Create and activate * a new `conda` [environment](http://conda.pydata.org/docs/using/envs.html).

\* Each time you wish to work on any exercises, activate your `conda` environment!

---

## 1. Installation

**Download** the latest version of `miniconda` that matches your system.

|        | Linux | Mac | Windows | 
|--------|-------|-----|---------|
| 64-bit | [64-bit (bash installer)][lin64] | [64-bit (bash installer)][mac64] | [64-bit (exe installer)][win64]
| 32-bit | [32-bit (bash installer)][lin32] |  | [32-bit (exe installer)][win32]

[win64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86_64.exe
[win32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86.exe
[mac64]: https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
[lin64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
[lin32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86.sh

**Install** [miniconda](http://conda.pydata.org/miniconda.html) on your machine. Detailed instructions:

- **Linux:** http://conda.pydata.org/docs/install/quick.html#linux-miniconda-install
- **Mac:** http://conda.pydata.org/docs/install/quick.html#os-x-miniconda-install
- **Windows:** http://conda.pydata.org/docs/install/quick.html#windows-miniconda-install

## 2. Create and Activate the Environment

For Windows users, these following commands need to be executed from the **Anaconda prompt** as opposed to a Windows terminal window. For Mac, a normal terminal window will work. 
## Getting Started

Follow the instructions in `starter_code/student_project.ipynb` and be sure to set up your Anaconda environment to get started!


### Dependencies
Using Anaconda consists of the following:

1. Install [`miniconda`](http://conda.pydata.org/miniconda.html) on your computer, by selecting the latest Python version for your operating system. If you already have `conda` or `miniconda` installed, you should be able to skip this step and move on to step 2.
2. Create and activate * a new `conda` [environment](http://conda.pydata.org/docs/using/envs.html).

\* Each time you wish to work on any exercises, activate your `conda` environment!

---

## 1. Installation

**Download** the latest version of `miniconda` that matches your system.

|        | Linux | Mac | Windows | 
|--------|-------|-----|---------|
| 64-bit | [64-bit (bash installer)][lin64] | [64-bit (bash installer)][mac64] | [64-bit (exe installer)][win64]
| 32-bit | [32-bit (bash installer)][lin32] |  | [32-bit (exe installer)][win32]

[win64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86_64.exe
[win32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Windows-x86.exe
[mac64]: https://repo.continuum.io/miniconda/Miniconda3-latest-MacOSX-x86_64.sh
[lin64]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86_64.sh
[lin32]: https://repo.continuum.io/miniconda/Miniconda3-latest-Linux-x86.sh

**Install** [miniconda](http://conda.pydata.org/miniconda.html) on your machine. Detailed instructions:

- **Linux:** http://conda.pydata.org/docs/install/quick.html#linux-miniconda-install
- **Mac:** http://conda.pydata.org/docs/install/quick.html#os-x-miniconda-install
- **Windows:** http://conda.pydata.org/docs/install/quick.html#windows-miniconda-install

## 2. Create and Activate the Environment

For Windows users, these following commands need to be executed from the **Anaconda prompt** as opposed to a Windows terminal window. For Mac, a normal terminal window will work. 

#### Git and version control
These instructions also assume you have `git` installed for working with Github from a terminal window, but if you do not, you can download that first with the command:
```
conda install git
```

If you'd like to learn more about version control and using `git` from the command line, take a look at our [free course: Version Control with Git](https://www.udacity.com/course/version-control-with-git--ud123).

**Now, we're ready to create our local environment!**

1. Clone the repository, and navigate to the downloaded folder. This may take a minute or two to clone due to the included image data.
```
git clone https://github.com/udacity/nd320-c1-emr-data-starter.git
cd nd320-c1-emr-data-starter
```

2. Create (and activate) a new environment, named `udacity-ehr-env` with Python 3.7. If prompted to proceed with the install `(Proceed [y]/n)` type y.

	- __Linux__ or __Mac__: 
	```
	conda create -n udacity-ehr-env python=3.7
	source activate udacity-ehr-env
	```
	- __Windows__: 
	```
	conda create --name udacity-ehr-env python=3.7
	activate udacity-ehr-env
	```
	
	At this point your command line should look something like: `(udacity-ehr-env) <User>:USER_DIR <user>$`. The `(udacity-ehr-env)` indicates that your environment has been activated, and you can proceed with further package installations.



6. Install a few required pip packages, which are specified in the requirements text file. Be sure to run the command from the project root directory since the requirements.txt file is there. I also added a line for installing the environment in your notebook in case this is new for you. You should be able to now look for the environment when you select the kernel.
 
```
pip install -r requirements.txt
ipython3 kernel install --name udacity-ehr-env --user

```



## License

This project is licensed under the MIT License - see the [LICENSE.md]()

#### Git and version control
These instructions also assume you have `git` installed for working with Github from a terminal window, but if you do not, you can download that first with the command:
```
conda install git
```

If you'd like to learn more about version control and using `git` from the command line, take a look at our [free course: Version Control with Git](https://www.udacity.com/course/version-control-with-git--ud123).

**Now, we're ready to create our local environment!**

1. Clone the repository, and navigate to the downloaded folder. This may take a minute or two to clone due to the included image data.
```
git clone https://github.com/udacity/AIHCND_C1.git
cd AIHCND_C1
```

2. Create (and activate) a new environment, named `udacity-ehr-env` with Python 3.7. If prompted to proceed with the install `(Proceed [y]/n)` type y.

	- __Linux__ or __Mac__: 
	```
	conda create -n udacity-ehr-env python=3.7
	source activate udacity-ehr-env
	```
	- __Windows__: 
	```
	conda create --name udacity-ehr-env python=3.7
	activate udacity-ehr-env
	```
	
	At this point your command line should look something like: `(udacity-ehr-env) <User>:AIHCND_C1 <user>$`. The `(udacity-ehr-env)` indicates that your environment has been activated, and you can proceed with further package installations.



6. Install a few required pip packages, which are specified in the requirements text file. Be sure to run the command from the project root directory since the requirements.txt file is there.
 
```
pip install -r requirements.txt
```

