NSfunc is an R package that leverages a variety of other R packages to 
provide analysis functions for NanoString data sets. By installing this
package, users have a streamlined, simplified way to run these analyses, 
and perhaps more importantly, a way to compare the results of these analyses
with further meta-analysis and visualization functions. More information
on NanoStringBionet can be found in the package vignette, which can be accessed once
the package is installed.

Installation Instructions:

Using the NS_Packrat bundle with R 3.5.1 and RStudio

This bundle contains all package dependencies required to run the NSfunc 
package in R 3.5.1, including NSdata (the NanoStringBionet class package)
and NSfunc (the analysis and reporting package).  To use this bundle,
first install the NS_packrat bundle to your local machine. Then, install 
packrat using the following command in RStudio:

install.packages("packrat")

Then use packrat to unbundle the project, replacing "path/to/bundle" with the
full file path of the bundle, including the full filename, and replacing 
"path/to/a/new/project" with the file path where you would like the project to
be unbundled to:

packrat::unbundle("path/to/bundle", "path/to/a/new/project")

You may get a fatal error from packrat about being unable to install NSdata, 
but it did not appear to actually be a problem during testing. Once the project 
is unbundled, switch to the new project by clicking on the "NS_Packrat.Rproj"
file (which should take the user to a new RStudio window), and load the NSfunc
package:

library(NSfunc)

Once the library is loaded, use the following command to access the package vignette:

browseVignettes("NSfunc")

Follow the instructions in the vignette, starting from the section titled "Preparing an NSdata object".
