# 3rd-party-msi-wrapper-package
 This example shows how to wrap a 3rd party MSI installer in an NIPM package.

## Create a WinInst Package

If the non-NI installer (e.g. non-NI drivers) contains .msi files, you can follow these instructions to create a “WinInst” package:

1. First, [assemble the directory structure and files for a WinInst Package](http://www.ni.com/documentation/en/ni-package-manager/latest/manual/assemble-wininst-package/).  To do this, you will need to create a [control file](http://www.ni.com/documentation/en/ni-package-manager/latest/manual/control-file-attributes/) and an optional [instructions XML file for WinInst packages](http://www.ni.com/documentation/en/ni-package-manager/latest/manual/instructions-xml-wininst-packages/).
2. [Build a package from the assembled directory using the the Command Line Interface](http://www.ni.com/documentation/en/ni-package-manager/latest/manual/build-package-using-cli/).

## Example Code
The "..\Source\3rd party installer" folder contains the directory structure for a WinInst package.  This example uses the Python 2.7.13 MSI installer file.  This example did not use an instructions file because there is only a single .msi file for this installer.

The "..\Source\Packages" folder contains the built package from running the `nipkg pack` command (step 2 above).
