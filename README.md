The GAP 4 package "PackageManager"
==================================

[![Build Status](https://travis-ci.org/gap-packages/PackageManager.svg?branch=master)](https://travis-ci.org/gap-packages/PackageManager)
[![Code Coverage](https://codecov.io/github/gap-packages/PackageManager/coverage.svg?branch=master&token=)](https://codecov.io/gh/gap-packages/PackageManager)

A basic collection of simple functions for installing and removing GAP packages,
with the eventual aim of becoming a full pip-style package manager for the GAP
system.

Example invocations:

    gap> LoadPackage("PackageManager");

    gap> InstallPackage("digraphs");

    gap> InstallPackage("https://github.com/gap-packages/Semigroups.git");

    gap> InstallPackage("https://www.gap-system.org/pub/gap/gap4/tar.gz/packages/mapclass-1.2.tar.gz");

    gap> RemovePackage("semigroups");

By default, verbose information about a command's progress is printed to the
screen.  To see less of this information, try using:

    gap> SetInfoLevel(InfoPackageManager, 1);

For more information on the features of PackageManager, see the documentation at
https://gap-packages.github.io/PackageManager/doc/chap1.html
or enter GAP and call, for example,

    gap> ?InstallPackage

Citing
------
Please cite this package as:

[Tor19]
M. Torpey,
PackageManager (GAP package),
Easily download and install GAP packages,
Version X.Y (20XX),
https://github.com/gap-packages/PackageManager.

Acknowledgements
----------------
PackageManager was partly created with funding from the OpenDreamKit project:
https://opendreamkit.org/

<table class="none">
<tr>
<td>
  <img src="http://opendreamkit.org/public/logos/Flag_of_Europe.svg" width="128">
</td>
<td>
  This infrastructure is part of a project that has received funding from the
  European Union's Horizon 2020 research and innovation programme under grant
  agreement No 676541.
</td>
</tr>
</table>
