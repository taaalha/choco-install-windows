# What is this

If you reinstall windows, all your installed softwares/packages are wiped away. 
You then have to reinstall them one by one. 

If you find this tedious, then here is the solution. 

Just update the `pacakges.config` file with the things you want to install, and it will install everything all 
at once. 

No need to do the tedious process step by step. 


## Install choco
Chocolatey is a windows package manager. You can install it from
```
https://chocolatey.org/install
```
# Install packages
To install packages, run
```
choco install packages.config --yes
``` 


To refresh env in your shell, do
```
Import-Module $env:ChocolateyInstall\helpers\chocolateyProfile.psm1 
```
and then
```
refreshenv
```
