# Instructions

- ### [Mac Installing `git`](#mac_installing_git)</br>
- ### [Windows Installing `git`](#win_installing_git)</br>
- ### [Accepting the assignment](#accepting_the_assignment)</br>
- ### [Cloning the assignment](#cloning_the_assignment)</br>
- ### [Project organization](#project_organization)</br>
- ### [Getting started with the project](#getting_started)</br>
- ### [Completing the project](#completing_the_project)</br>

---

</br>

<a name="mac_installing_git"></a>

## Mac Installing git

We use [homebrew](https://brew.sh/) to [install git](https://git-scm.com/download/mac).

```sh
$ brew install git
```

If you see "brew: command not found", then you need to install brew.

```sh
$ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# The following two lines for Apple M1 Processor

# you can find the following command in terminal
$ echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/YOUR_DEVICE_NAME/.zprofile

$ eval $(/opt/homebrew/bin/brew shellenv)
```

You need to install **Xcode** from App Store before you use other IDE.

### Check git installation

To make sure git is installed correctly

```sh 
$ git --version
```

<img src="images/mac_images/b-00-git_version.png" alt="git version" width="1000"/>

</br>

### Login git

Login git with username and email address:

```sh
$ git config --global user.name "stephengineer"
$ git config --global user.email "swang03@pasadena.edu"
```

---

</br>

<a name="win_installing_git"></a>

## Windows Installing git

### Download `git`

Download git from [here](https://git-scm.com/download/win). You should get an exe similar to this: `Git-2.30.0.2-64-bit.exe`

<img src="images/win_images/git-01-download_git_00.png" alt="download_git" width="1000"/>

</br>

### Install `git`

Open/Run the executable file, and follow the steps to install.

Choose Default.

<img src="images/win_images/git-01-download_git_01.png" alt="download_git" width="1000"/>

</br>

Choose Git Credential Manager Core.

<img src="images/win_images/git-01-download_git_02.png" alt="download_git" width="1000"/>

</br>

Select Only show new options if not selected, and click next.

<img src="images/win_images/git-01-download_git_03.png" alt="download_git" width="1000"/>

Choose Let git decide.

<img src="images/win_images/git-01-download_git_04.png" alt="download_git" width="1000"/>

</br>

Choose Use OpenSSH.

<img src="images/win_images/git-01-download_git_05.png" alt="download_git" width="1000"/>

</br>

Choose Default (fast-forward or merge).

<img src="images/win_images/git-01-download_git_06.png" alt="download_git" width="1000"/>

</br>

Choose Git Credential Manager Core

<img src="images/win_images/git-01-download_git_07.png" alt="download_git" width="1000"/>

</br>

And Install!

<img src="images/win_images/git-01-download_git_08png.png" alt="download_git" width="1000"/>

<img src="images/win_images/git-01-download_git_10.png" alt="download_git" width="400"/>

<img src="images/win_images/git-01-download_git_11.png" alt="download_git" width="400"/>

</br>

When it is done installing, click Finish.

<img src="images/win_images/git-01-download_git_12.png" alt="download_git" width="1000"/>

</br>

You may view release notes if you want.

<img src="images/win_images/git-01-download_git_13.png" alt="download_git" width="1000"/>

</br>

### Check git installation

To make sure git is installed correctly

```sh 
$ git --version
```

<img src="images/win_images/git-02-git_version.png" alt="download_git" width="1000"/>

<br/>

### Login git

Login git with username and email address:

```sh
$ git config --global user.name "stephengineer"
$ git config --global user.email swang03@pasadena.edu
```

---

</br>

<a name="accepting_the_assignment"></a>

### Accepting the assignment

Here is the **assignment link** for [CS2](https://github.com/stephengineer-CS002-classroom/CS2_Assignments).

### Accept assignment

1. Click on the accept assignment link.
1. Select yourself from the list with your name.
1. Click on the green button, `Accept this assignment`  to accept the assignment.

<img src="images/others/a-00-accept_assignment.png" alt="accept_assignment" width="1000"/>


</br>

This will create a repo under your github username. The name of repo will be the name of assignment followed by your github name.

> `00_lab_0-stephengineer`

</br>

### Assignment repo

Once you accepted the assignment, github will begin to create your assignment repo and give it a few seconds, then:

1. Refresh this page to see updates.
1. Click the link of repo.

<img src="images/others/a-04-refresh_to_update.png" alt="refresh_to_update" width="1000"/>

<img src="images/others/a-04-reload_to_update.png" alt="reload_to_update" width="1000"/>

</br>

__Note__: Bookmark this page to know how to get here. We'll need to check in here soon.

<img src="images/others/a-06-your-repo.png" alt="your-repo" width="1000"/>

---

</br>

<a name="cloning_the_assignment"></a>

### Get git link of assignment

1. Click on the green `Code` button on the mid-right.
1. Click the little clipboard and that will copy the link into your clipboard so you can paste it in the next step. 

<img src="images/others/a-07-copy_clone_link.png" alt="copy_clone_link" width="1000"/>

</br>

### Clone assignment

Before you can work on your project, you will need a local copy of the assignment. This is called **clone** the repository.

```sh
# create and go the the directory of projects
$ cd /Users/stephen/CS2/

# clone repo
$ git clone https://github.com/stephengineer-CS002-classroom/00_lab_0-stephengineer.git
```

---

</br>

<a name="project_organization"></a>

### Open assignment with IDE

For example, open VSCode and loads the project folder

```sh
# go the project folder
$ cd 00_lab_0-stephengineer

# open VSCode
$ code .
```

</br>

### File system

All the projects in this class will follow the same file organization.

On the left panel (Explorer) you will find:

- `main.cpp`: on the root folder, this will be the most important file you finish assignment before you learn function.

- `includes`: contains a folder for the function your project depends on. In this starter code, you only have a `stub` folder that contains `stub.h` and `stub.cpp`. These files are `#include`d in `main.cpp`

- `submit.sh`: run `sh submit.sh` to submit your assignment to github to get grader.

<img src="images/others/02-vscode_file_structure.png" alt="vscode_after_cloning" width="200"/>

---

</br>

<a name="getting_started"></a>

### Step 1: Find `main.cpp`

For some assignments, I will create the `basic_test` function to demonstrate the functionality of the project and for you to make sure that your code match the grader's expectations. (otherwise, your projects will not earn a score.)

You will copy this `main.cpp` and overwrite the existing _generic_ `main.cpp` in your project folder. After this, you will __NEVER__ edit the `basic_test` function.

Pay special attention to the `#include` path at the top. Your file structure has to be __exactly__ the same as the one depicted here.

<br>

### Step 2: Create project folder

Create a new function folder under the `includes/` folder and name this folder by instruction of assignment. This is the directory you will add your `.h` and `.cpp` files.

### Step 3: Add two project files

Add two files in the project folder:

- `xxx.h`
- `xxx.cpp`

</br>

### Step 4: Add the function signatures

Add these function signatures to the `xxx.h`

### Step 5: Open terminal

If you are using VSCode, you can open the terminal by pressing [`ctrl`]+[ ` ]

[`] is the key in the top left of the keyboard

Using the terminal in this way is very convenient.

</br>

### Step 6: Build project

</br>

### Step 7: Compile project

Now, we are ready to compile project by clicking on **Run** (triangle) button.

</br>

### Step 8: Push changes to Github

Run git commands to commit changes:

To open the terminal by pressing [`ctrl`]+[ ` ]

#### Mac
```sh
$ sh submit.h

# input some comments for your current change and press enter, for example.
Comments of Submission: init changes
```

#### Windows
```sh
$ ./submit.h

# input some comments for your current change and press enter, for example.
Comments of Submission: init changes
```

---

</br>

<a name="completing_the_project"></a>

## Autograder Status

You can keep track of the grading status of your project on the assignment page. A yellow dot means that the tests are still being compiled and run by the autograder. This shouldn't take more than a minute or two. You can refresh the page to update the status. A green checkmark means that all your tests have passed. A red x means that at least one test failed.

<br/>

Yellow dot: running autograder

<img src="images/others/test-04_results_github_01.png" alt="test_result_github" width="1000"/>

</br>

A red x: at least one test failed

<img src="images/others/test-04_results_github_02.png" alt="test_result_github" width="1000"/>

</br>

A green checkmark: all tests have passed

<img src="images/others/test-04_results_github_03.png" alt="test_result_github" width="1000"/>

</br>

Click on `Details` to see test details.

<img src="images/others/test-04_results_github_04.png" alt="test_result_github" width="1000"/>