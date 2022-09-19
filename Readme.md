# Trashy Missing Data Tutorial for Trash Pandas and Friends
The tutorial here is a light adaption of example code from the [numpyro](https://github.com/pyro-ppl/numpyro)  package with data supplied from the [WiDS Datathon 2020](https://www.kaggle.com/competitions/widsdatathon2020/data). While initial purpose of the example code was to demonstrate how MCMC can be used to impute binary variables, we've adapted it to demonstrate how assumptions about missingness affect model parameters. The tutorial was tested on our (Pat's) laptop, and our (Earlyn's) GCP virtual machine. The code runs at an unannoyingly pace in both environments.

### Environment Setup
To run the tutorial you will need to jupyter working with the appropriate packages install. If you already have python 3.9 installed on your machine, you can skip steps 1 and 2.


1. Clone or dowload this repo
If you don't currently have git, get it at https://git-scm.com/downloads if you would like to clone this repo. If you would prefer to simply download the code, click the green code button above and go to download zip.


2. Download Python Installer
Go to [Python 3.9.13](https://www.python.org/downloads/release/python-3913/) and download the installer appropriate for your system. We choose Python 3.9 for compatibility with the packages used in the tutorial, rather than using the most recent stable release, 3.10. 


3. Install Python
Run the downloaded installer. The default setting should suffice.


4. Download and install Graphviz
You will find installer at https://graphviz.org/download/. The most recent version for you system should be compatible with the tutorial. This isn't strictly necessary, but if you'd like to see the directed graphs used to visualize the simulations, you will want this.


5. Install requirement
Open a cmd shell, powershell... shell I guess, or terminal. navigate to where you have placed this directory on your system and run:
`pip install -r req.txt`
I you have pip troubles, check out [Using Python's pip to Manage Your Projects' Dependencies](https://realpython.com/what-is-pip/#getting-started-with-pip), and hopefully it will see you through. The current req.txt file is setup specifically for Windows. If you are running this in another environment, you will need to edit the req.txt removing the content prior to the jax package [here](https://github.com/mediwareinc/TrashyMissingDataTutorial/blob/93c54a4b9d3789cf7454fc3777fd71048affaab2/req.txt#L16) 


6. Start the jupyter notebook server
After the requirements have been installed using pip, run:
`jupyter notebook`. This should start a server in the terminal, shell, console, etc., and open a page to your local notebook server in your favorite browser, unless of corse that's something odd like Opera, or Safari, or something like that... not sure if those are compatible.


7. Run the notebook
Click on discrete_imputation.ipynb and let the full force of this tutelage overcome you.
