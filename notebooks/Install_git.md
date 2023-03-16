---
fig-cap-location: top
from: markdown+emoji
---

# **Install Git**

<div class="questions">

### **Questions** {.unlisted}
* Have you installed `Git` on your system?
</div>
</br>

You need Git, so you can use it at the command line and so RStudio can call it.

To check if git is installed, enter the following command in your command-line to request the path to your Git executable:
```default
which git
## /usr/bin/git
```
<br>
and git --version to see its version:
```default
git --version
## git version 2.39.1
```



If either/or both the command do not generate results similar to above,instead, you see something more like 
```default
git: command not found, 
```
<br> please proceed to install git by following the instructions appropriate to your operating system.



::: {.callout-note}
**macOS** users might get an immediate offer to install command line developer tools. Yes, you should accept! Click `Install` and read more below.
:::

## **Windows**

**Option 1** (highly recommended): Install Git for Windows, also known as `msysgit` or `Git Bash`, to get Git in addition to some other useful tools, such as the Bash shell.

THis option to insatll git is recommended because Git for Windows leaves the Git executable in a conventional location, which will help you and other programs, e.g. RStudio, find it and use it. This also supports a transition to more expert use, because the 'Git Bash' shell will be useful as you venture outside of R/RStudio.

**NOTE**: When asked aboutAdjusting your PATH environment, make sure to select `Git from the command line and also from 3rd-party software`. Otherwise, we believe it is good to accept the defaults.
Note that RStudio for Windows prefers for Git to be installed below `C:/Program Files` and this appears to be the default. This implies, for example, that the Git executable on my Windows system is found at `C:/Program Files/Git/bin/git.exe`. Unless you have specific reasons to otherwise, follow this convention.


**Option 2** (recommended): Install Git for Windows via the 'Chocolatey' package manager. 
<br>Chocolatey is like `apt-get` or `Homebrew`, but for Windows instead of Debian/Ubuntu Linux or macOS. Using Chocolatey to install Git for Windows gives the same result as installing it yourself using 'Option 1'.

This requires that you already have `Chocolatey` installed or that you are up for installing it. The instructions for installing `Chocolatey` are [here](https://chocolatey.org/install). This may be worthwhile if it seems likely you will be installing more open source software in the future.

After you install Chocolatey, in a shell (Appendix A), do:

```default
choco install git.install
```
<br>This installs the most current Git (Install) X.Y.Z Chocolatey package. At the time of writing, that is `Git (Install) 2.33.1`, but that version number will increment over time.

### Updating Git for Windows
<br>If you already have Git for Windows, but it’s not the latest version, it’s a good idea to update. Since v2.16, you can update like so from the command line:
```default
git update-git-for-windows
```


## **macOS**

**Option 1** (highly recommended): Install the Xcode command line tools (not all of Xcode), which includes Git.
<br>Go to the shell and enter one of these commands to elicit an offer to install developer command line tools:

```default
git --version
git config
```
<br> Accept the offer! Click on `Install`.

<br>
Here’s another way to request this installation, more directly:
```default
xcode-select --install
```


**Option 2** (recommended): Install Git from [here](http://git-scm.com/downloads)

<br>This method will certainly get you the latest version of Git of all approaches described here.
<br>The GitHub home for the macOS installer is [here](https://github.com/timcharper/git_osx_installer). At that link, you can find more info if something goes wrong or you are working on an old version of macOS.

**Option 3** (recommended): If you anticipate getting heavily into scientific computing, you’re going to be installing and updating lots of software. You should check out [Homebrew](https://brew.sh/), “the missing package manager for OS X”. Among many other things, it can install Git for you. Once you have Homebrew installed, do this in the shell:

```default
brew install git
```


## **Linux**
Install Git via your distro’s package manager.

Ubuntu or Debian Linux:
```default
sudo apt-get install git
```
Fedora or RedHat Linux:

```default
sudo yum install git
```
<br> Click [here](https://git-scm.com/download/linux) for a comprehensive list for various Linux and Unix package managers.




<div class="challenge">

</div>  

</br>



<div class="keypoints">

### **Key points** {.unlisted}


</div>  



  
