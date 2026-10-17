

*This project has been created as part of the 42 curriculum by hrazafia*

## Description

`ft_package` is a simple Python package that provides utility functions for working with lists. It provides the `count_in_list()` function, which counts the number of occurrences of an item in a list.

## Instructions

#### Build

Clone the repository and navigate to the project directory:

```bash
git clone git@github.com:hrazafia/ft_package.git ft_package
cd ft_package
```

Build the package:

```bash
python -m build
```

This command generates two distribution files in the `dist/` directory:

- `ft_package-0.0.1.tar.gz` — source distribution.
- `ft_package-0.0.1-py3-none-any.whl` — wheel distribution.

#### Installation

Install the wheel distribution:

```bash
python -m pip install ./dist/ft_package-0.0.1-py3-none-any.whl
```

Alternatively, install the source distribution:

```bash
python -m pip install ./dist/ft_package-0.0.1.tar.gz
```

#### Uninstallation

To uninstall `ft_package`, run:

```bash
python -m pip uninstall ft_package
```

Confirm the uninstallation when prompted.


## Usage

Import `count_in_list()` from the package:

```python
from ft_package import count_in_list

print(count_in_list(["toto", "tata", "toto"], "toto"))
print(count_in_list(["toto", "tata", "toto"], "tutu"))
```

Output:

```text
2
0
```

The function returns the number of occurrences of the specified item in the list.

## Function

### `count_in_list(lst, item)`

**Parameters:**

- `lst`: The list to search.
- `item`: The item whose occurrences are counted.

**Returns:**

- `int`: The number of occurrences of `item` in `lst`.

**Example:**

```python
count_in_list(["a", "b", "a", "c", "a"], "a")
# Returns 3
```

## Resources

- [Learn Python Programming, Fourth Edition — Packt Publishing](https://www.packtpub.com/en-us/product/learn-python-programming-9781835882948)
- [The MIT License — Open Source Initiative](https://opensource.org/license/mit)
- AI has been used to help understand the process of developing Python packages, including project structure, configuration via `pyproject.toml`, as well as the building, distribution, and installation of packages.
