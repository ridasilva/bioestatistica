# Bioestatística 

<p align="center">
  <img src="https://github.com/ridasilva/bioestatistica/blob/master/img/logo.png" alt="logo"/>
</p>

## Installation

Install conda

```
wget https://repo.continuum.io/miniconda/Miniconda2-latest-Linux-x86_64.sh
bash Miniconda2-latest-Linux-x86_64.sh

```
   
Create a dedicated conda environment and activate

```
conda env create -f environment.yml
conda activate bioestats 
```

If a new library needs to be installed, don't forget to update the environment.yml file 

```
conda env export | grep -v "^prefix: " > environment.yml 
```

### Building jupyter-book

Build

```
jupyter-book build bioestatistica/
```

You can preview the result on `_build/html/index.html` 