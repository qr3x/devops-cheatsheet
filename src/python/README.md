# Python

## Content
1. Init env: [`Create env`](#create-environment), [`Activate env`](#activate-environment), [`Install libraries`](#install-libraries)
2. Conditional operator `if`: [`Conditional operator if`](#conditional-operator-if), [`Ternatry if`](#ternary-if)

## Create environment  
Template:
```bash
python -m venv <env name> 
```
Example:
```bash
python -m venv venv
```

## Activate environment
* Unix  
  Template:
  ```bash
  source <env name>/bin/activate
  ```
  Example
  ```bash
  source venv/bin/activate
  ```

* Windows  
  Template:
  ```bash
  <env name>\Scripts\activate.bat
  ```
  Example:
  ```bash
  venv\Scripts\activate.bat
  ```

## Install libraries
1. Install libraries from [PyPi](https://pypi.org/)  
   Template:
   ```bash
   pip install <1st library> <2nd library> <etc>
   ```
   Example:
   ```bash
   pip install loguru numpy
   ```

2. Install libraries from the private repository  
   Template:
   ```bash
   pip install -i <private repo url> <1st library> <2nd library> <etc>
   ```
   Example:
   ```bash
   pip install -i https://pypi.python.org/simple loguru numpy
   ```

3. Install libraries using the `reqirements.txt` file  
   Template:
   ```bash
   pip install -r <file>
   ```
   Example:
   ```bash
   pip install -r reqirements.txt
   ```

## Main
Runs main() if file wasn't imported
```python
if __name__ == '__main__':
    main()
```

## Conditional operator `if`
1. Regular `if`  
   Template:
   ```python
   if <condition 1>:
     <code>
   elif <condition 2>:
     <code>
   else:
     <code>
   ```
   Example:
   ```python
   age = 15
   if age > 21:
     print('Adult in Argentina')
   elif age > 18:
     print('Adult in Russia')
   else:
     print('Not an adult')
   ```

2. Ternary `if`  
   Template:
   ```python
   <condition is True> if <condition> else <condition is False>
   ```
   Examples:
   ```python
   age = 15
   print('Adult') if age > 18 else print('Not an adult')
   ```
   ```python
   is_cat = True
   animal = 'cat' if is_cat else 'dog'
   ```
