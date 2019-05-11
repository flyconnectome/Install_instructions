# Installation instructions for Anaconda3 Navigator on linux x86_64 machines at Janelia.

Due to user permissions and potential machine breaks on the linux machines at Janelia, 
one of two methods for updating python, pip etc. is to use the [Anaconda platform](www.anaconda.org). 

These instructions are specified for downloading Anaconda3-2019 on a x86_64 Linux machine, although these 
instructions can me modified to download and install any version of Anaconda3 or Anaconda2 
from the [anaconda online archive](https://repo.anaconda.com/archive/) 

This install will also update pip. 

## Install instructions

1. Remove older versions.

If you already have a version of anaconda3 or anaconda2 installed on your computer, then I suggest
removing these installations before proceeding - if they were working, you wouldn't be here. 

Open the terminal and run:

``` 
rm -rf ~/anaconda3
```

Substitue anaconda3 for anaconda2 as needed.

1. Download Anaconda

Move our current working directory to the tmp folder (temporary folder), 
so that the install files get deleted after we've installed and turned our 
computer on after a long hard day of installing anaconda3

```
cd /tmp/
```

Download the installation file.


```
wget https://repo.anaconda.com/archive/Anaconda3-2019.03-Linux-x86_64.sh
```

Note: the `Anaconda3-2019.03-Linux-x86_64.sh` path can be substituted for any 
version of anaconda on the [anaconda repo](https://repo.anaconda.com/archive/)


1. Install on Ubuntu

Start the install

```
bash Anaconda3-2019.03-Linux-x86_64.sh
```

This will show the USER AGREEMENT in the terminal, which must be agreed to. There will be 
a specific prompt asking you whether you agree to this agreement. Simply type `yes`.

You will see a list of core packages being installed. 

After this, there will be prompt asking you whether to terminate the conda-init file.
Agree to this and close the terminal. 

1. Test

Now to open anaconda we have two options, both of which must be entered in a new terminal window.

	1. Open anaconda navigator and install the desired platforms
	
... Enter `anaconda-navigator` into the terminal. This will load the anaconda-navigator 
... platform management (you should see a large green circle in the middle of your screen)
...	Download the packages you need (e.g. Jupyter notebook, Jupyter lab, R, Spyder)

	1. Just open Jupyter notebook/ lab
	
	
... `jupter notebook`
... OR
... `jupyter lab`


## WOOP! Anaconda should be downloaded and now you can start installing 
the packages you need like [dvid_tools](https://github.com/flyconnectome/dvid_tools), 
[pymaid](https://pymaid.readthedocs.io/en/latest/) and [neuprint_python](https://neuprint-python.readthedocs.io/en/latest/) 



# Acknowledgements / Requiring further assistance 

These instructions were written by Markus Pleijzier, RA at the Drosophila Connectomics Group, Department of Zoology, University of Cambridge.

If you need further assistance please don't hesitate to contact Markus. He is available on the FlyEM slack channel.






