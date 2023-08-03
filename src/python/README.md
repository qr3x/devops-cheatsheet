# Python

## Content
Init env: [`Create env`](#create-environment), [`Activate env`](#activate-environment), [`Install libraries`](#install-libraries)

## Create environment
```bash
python -m venv <env name> 
```
```bash
python -m venv venv
```

## Activate environment
* Unix
```bash
source <env name>/bin/activate
```
```bash
source venv/bin/activate
```

* Windows
```bash
<env name>\Scripts\activate.bat
```
```bash
venv\Scripts\activate.bat
```

## Install libraries
1. Install libraries from [PyPi](https://pypi.org/)
```bash
pip install <1st library> <2nd library> <etc>
```
```bash
pip install loguru numpy
```

2. Install libraries from the private repository
```bash
pip install -i <private repo url> <1st library> <2nd library> <etc>
```
```bash
pip install -i https://pypi.python.org/simple loguru numpy
```

3. Install libraries using the `reqirements.txt` file
```bash
pip install -r <file>
```
```bash
pip install -r reqirements.txt
```
