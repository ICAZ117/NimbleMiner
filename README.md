# NimbleMiner
NimbleMiner: a software that allows clinicians to interact with word embedding models (skip-gram models- word2vec and Glove) to rapidly create lexicons of similar terms.

# Windows Installation
1. Install base software:
   * [Download](https://cran.r-project.org/bin/windows/base/old/4.0.2/R-4.0.2-win.exe) and install R version 4.0.2
   * [Download](https://s3.amazonaws.com/rstudio-dailybuilds/RStudio-1.1.447.zip) and install/unzip RStudio version 1.1.447
   * [Download](https://cran.r-project.org/bin/windows/Rtools/rtools40-x86_64.exe) and install Rtools version 4.0
3. Restart your computer
4. Launch RStudio v1.1.447
   * Ensure RStudio is running R v4.0.2
      * Tools > Global Options > General > R Version > Change
      * In the "Choose R Installation" window that pops up, select the "Choose a specific version of R" option, and then select the 64 bit version of R v4.0.2
5. Manually install shiny and devtools from CRAN using the following commands:
   * ```
     install.packages("shiny", repos="http://cran.rstudio.com/", dependencies=TRUE)
     ```
   * ```
     install.packages("devtools", repos="http://cran.rstudio.com/", dependencies=TRUE)
     ```
6. From the cloned NimbleMiner repository, open installer/installer.R in RStudio
7. Begin the NimbleMiner installation by clicking the "Source" button (top right)
   * Note: This is \*different\* from the "Run" button
8. In the pop-up window asking if you want to download packages from source, click Yes
   * This window may/will show up several times during this installation proces. Always click yes.
9. Once the source installation is complete, restart RStudio
10. In the console, one at a time, run the following manual package installations
   * ```
     urlPackage <- "https://cran.r-project.org/src/contrib/Archive/randomForest/randomForest_4.6-14.tar.gz"
     install.packages(urlPackage, repos=NULL, type="source") 
     ```
   * ```
     urlPackage <- "https://cran.r-project.org/src/contrib/Archive/Matrix/Matrix_1.5-3.tar.gz"
     install.packages(urlPackage, repos=NULL, type="source")
     ```
   * ```
     install.packages("RTextTools", repos="http://cran.rstudio.com/", dependencies=TRUE)
     ```
   * ```
     install.packages("lava", repos="http://cran.rstudio.com/", dependencies=TRUE)
     ```
   * ```
     install.packages("text2vec", repos="http://cran.rstudio.com/", dependencies=TRUE)
     ```
   * ```
     install.packages("tokenizer", repos="http://cran.rstudio.com/", dependencies=TRUE)
     ```
11. Once these packages installations are complete, restart RStudio
12. Open NimbleMiner.R in RStudio and run it using the "Run App" button on the top right

# Generic Installation Guide
1. Copy all files and folders from NimbleMiner repository
2. Install base software:
* [Download](https://cran.r-project.org/) and install the last version of R (3.5.0 or later)
* [Download](https://www.rstudio.com/products/rstudio/download/#download) and install the last version of RStudio (1.1.447 or later)
* Download and install devtools:: 
   * On windows: [Rtools](https://cran.r-project.org/bin/windows/Rtools/) (35 or last recommended version) - Change the default path ( C:\RBuildTools ) to C:\Rtools
   * On Mac: [Xcode command line tools](https://developer.apple.com/downloads).
2. Restart the computer.

3. Install packages:  

* Open script installer/installer.R in RStudio  
* Run script with help of button "Source"
* Wait till all packages will be installed
* Restart R session (or restart RStudio)

4. Open NimbleMiner.R in RStudio and run it by the button "Run App"
