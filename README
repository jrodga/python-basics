# Python

# Variables

- A variable is a named reference to a value. Names are case-sensitive.

- Each variable holds one value at a time, but that value can be a container (e.g. list, dict).

- You can check a value’s type with type(x).

```python

age = 28
name = "Jonathan"
pi = 3.14159

type(age)    # <class 'int'>
type(name)   # <class 'str'>
type(pi)     # <class 'float'>

```

Good practice: use `snake_case` names; be descriptive: `daily_clicks`, not `dc`.

## List

A list is an ordered collection of items 

```python

numbers = [10, 20, 30]
mixed   = [1, "two", 3.0]

```
- Lists can hold any type, including mixed types.

- **Indexing** Access a single list item by position (0-based) and negative indexing (from the end):
```python

numbers[0]   # 10
numbers[-1]  # 30

```

**Subsetting & slicing**

take part of a list with `list[start:stop:step]`; start is inclusive, stop is exclusive.

```python

items = ["a", "b", "c", "d", "e"]
items[1:4]   # ['b', 'c', 'd']  (start inclusive, stop exclusive)
items[:3]    # ['a', 'b', 'c']
items[3:]    # ['d', 'e']
items[::2]   # step: ['a','c','e']

```
**List manipulation**

Change, add, or remove elements using assignment, `append`, `extend`, `del`, or `remove`.

```python

items[2] = "X"
items.append(99)
items.extend([7,8])
del items[0]
items.remove("X")

```
##
## Dictionaries 

- Key–value maps with unique, immutable keys for fast lookups and updates.
```python

person = {"name": "Sam", "age": 30}

```
**Dictionary lookups**

- Retrieve values by key via `d[key]` or safely with `d.get(key, default)`.

```python

person["name"]           # 'Sam'
person.get("city","N/A") # 'N/A'


```
**Add/remove in dicts**

- Set `d[new_key] = value` to add/update; `del d[key]` to delete.
```python

person["role"] = "Analyst"
del person["age"]

```
##
## Functions
- Reusable blocks of code defined with `def` that take inputs and return results.

```python

def ctr(clicks, impressions):
    return clicks / impressions if impressions else None

```
**Packages & modules**
- Installable collections of Python code; import to gain extra functions and types.

in a terminal (bash)
```bash

python -m pip install numpy pandas matplotlib

```
in a Python environment
```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt

```
##
## NumPy
- NumPy arrays: Fixed-type, fast numeric containers enabling vectorised maths over whole arrays.

```python

import numpy as np
a = np.array([1,2,3,4])
a.mean()       # 2.5
a * 10         # array([10,20,30,40])

```
##
## Pandas
- DataFrame: Table-like structure with labelled rows/columns for organising and analysing data. (df = abbreviation of data frame)

```python

import pandas as pd
df = pd.DataFrame({"country":["BR","RU"], "capital":["Brasília","Moscow"]})

```
**Bracket selection (pandas)**
- `df["col"]` for a Series, `df[["a","b"]]` for multiple columns, `df[i:j]` to slice rows.

```python

df["country"]
df[["country","capital"]]
df[0:1]

```
**`loc` (label-based)**
Definition: Select rows/columns by their labels (names), e.g. `df.loc[labels, cols]`.

```python

df.loc[:, ["country","capital"]]

```

**`iloc` (position-based)**
- Select rows/columns by integer positions, e.g. `df.iloc[rows, cols]`.

python
Copy code
df.iloc[:, [0,1]]
