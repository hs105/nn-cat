# nn-cat

# required packages
* python 3.7
* tensorflow 2.0
* gym 0.15.4

I used conda to install all the packages. 
```
conda create --name tf1.15 tensorflow=1.15 python=3.7
conda activate tf1.15
git clone https://github.com/openai/gym.git
cd gym
pip install -e .
```
The last step may have a problem. Double check if you have all the packages in the virtual env.
``` 
conda list
```
If not, the pip command may be linked to the global system pip. Try using 
```
which pip
```
Based on the result, use 
```
/Users/dongcui/opt/anaconda3/envs/tf1.15/bin/pip install -e .
```
Do "conda list" again, you should have all the required packages installed. 

# Setup Pycharm working environment
I used pycharm as python editor. 

* Open the working directory of this project using pycharm, set the project interpreter to use the conda environment we've just created. 
* Choose "Conda environment", "Existing environment", and locate the python interpreter in the directory of the conda environment.  






# reference:
* [Dropout](http://jmlr.org/papers/v15/srivastava14a.html)
