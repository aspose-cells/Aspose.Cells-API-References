---
title: replace method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 330
url: /python-net/aspose.cells/workbook/replace/
is_root: false
---

## replace(place_holder, new_value) {#str-str}

Replaces a cell's value with a new string.



```python
def replace(self, place_holder, new_value):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | str | Cell placeholder |
| new_value | str | String value to replace |

### Example 


```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
workbook.replace("AnOldValue", "NewValue")

```


## replace(place_holder, new_value) {#str-int}

Replaces a cell's value with a new integer.



```python
def replace(self, place_holder, new_value):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | str | Cell placeholder |
| new_value | int | Integer value to replace |

### Example 


```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100
workbook.replace("AnOldValue", newValue)

```


## replace(place_holder, new_value) {#str-float}

Replaces a cell's value with a new double.



```python
def replace(self, place_holder, new_value):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | str | Cell placeholder |
| new_value | float | Double value to replace |

### Example 


```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValue = 100.0
workbook.replace("AnOldValue", newValue)

```


## replace(bool_value, new_value) {#bool-any}

Replaces cells' values with new data.



```python
def replace(self, bool_value, new_value):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| bool_value | bool | The boolean value to be replaced. |
| new_value | any | New value. Can be string, integer, double or DateTime value. |


## replace(int_value, new_value) {#int-any}

Replaces cells' values with new data.



```python
def replace(self, int_value, new_value):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| int_value | int | The integer value to be replaced. |
| new_value | any | New value. Can be string, integer, double or DateTime value. |


## replace(place_holder, new_values, is_vertical) {#str-list-bool}

Replaces a cell's value with a new string array.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | str | Cell placeholder |
| new_values | list | String array to replace |
| is_vertical | bool | True - Vertical, False - Horizontal |

### Example 


```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = ["Tom", "Alice", "Jerry"]
workbook.replace("AnOldValue", newValues, True)

```


## replace(place_holder, new_values, is_vertical) {#str-list-bool}

Replaces cells' values with an integer array.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | str | Cell placeholder |
| new_values | list | Integer array to replace |
| is_vertical | bool | True - Vertical, False - Horizontal |

### Example 


```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1, 2, 3]
workbook.replace("AnOldValue", newValues, True)

```


## replace(place_holder, new_values, is_vertical) {#str-list-bool}

Replaces cells' values with a double array.



```python
def replace(self, place_holder, new_values, is_vertical):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | str | Cell placeholder |
| new_values | list | Double array to replace |
| is_vertical | bool | True - Vertical, False - Horizontal |

### Example 


```python
from aspose.cells import Workbook

workbook = Workbook()
# ......
newValues = [1.23, 2.56, 3.14159]
workbook.replace("AnOldValue", newValues, True)

```


## replace(place_holder, new_value, options) {#str-str-ReplaceOptions}

Replaces a cell's value with a new string.



```python
def replace(self, place_holder, new_value, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | str | Cell placeholder |
| new_value | str | String value to replace |
| options | [ReplaceOptions](/cells/python-net/aspose.cells/replaceoptions) | The replace options |



### See Also
* module [aspose.cells](../../)
* class [Workbook](/cells/python-net/aspose.cells/workbook)
