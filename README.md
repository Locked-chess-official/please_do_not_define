# please_do_not_define
Python library that prevents you from defining variables, functions or classes with names that contain female-related terms.
Now that a small number of women declare that they are undefinedable. The library will make sure that you won't offend them.
![IDLE Shell 3 13 5 2025_6_15 15_11_30](https://github.com/user-attachments/assets/84e97919-4842-4b3c-a809-8f32f9e2aa86)


## Installation

`pip install please_do_not_define`

## Purpose

This library helps maintain gender-neutral naming in your Python code by detecting and blocking the use of female-related terms in variable, function, and class names.

## Features
- Scans Python code for names containing female-related terms

- Blocks execution if prohibited names are found

- Supports detection of both English and Chinese female-related terms

- Works with various file encodings

## Usage

Simply import the library in your Python script:

`import please_do_not_define`

The library will automatically scan your main script file when imported and raise a NameError if any prohibited names are found.

## Prohibited Terms

The library checks for names containing any of the following terms (case insensitive):

- Chinese Terms:

`女, 姑, 婆, 媳, 妇, 娘, 嬷, 姐, 妹, 嬢, 媛`

- English Terms:

`woman, women, girl, lady, Miss, Mrs, queen, female, she, her`

## Example

If your code contains:
```
def print_girl_name():
    pass
```

The library will raise:

`NameError: name 'print_girl_name' is illegal. Please don't try to define a female.`

## Note

This library is intended to satirize a concept, not the actual effect.

## License

MIT
