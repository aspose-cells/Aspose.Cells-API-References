##replace method
## replace(self, place_holder, new_value) {#System.String-System.String}
Replaces a cell's value with a new string.
```python
def replace(self, place_holder, new_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | System.String | Cell placeholder |
| new_value | System.String | String value to replace |
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
# ......
workbook.replace("AnOldValue", "NewValue")
```
## replace(self, place_holder, new_value) {#System.String-int}
Replaces a cell's value with a new integer.
```python
def replace(self, place_holder, new_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | System.String | Cell placeholder |
| new_value | int | Integer value to replace |
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
# ......
newValue = 100
workbook.replace("AnOldValue", newValue)
```
## replace(self, place_holder, new_value) {#System.String-float}
Replaces a cell's value with a new double.
```python
def replace(self, place_holder, new_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | System.String | Cell placeholder |
| new_value | float | Double value to replace |
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
# ......
newValue = 100.0
workbook.replace("AnOldValue", newValue)
```
## replace(self, bool_value, new_value) {#bool-System.Object}
Replaces cells' values with new data.
```python
def replace(self, bool_value, new_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| bool_value | bool | The boolean value to be replaced. |
| new_value | System.Object | New value. Can be string, integer, double or DateTime value. |
## replace(self, int_value, new_value) {#int-System.Object}
Replaces cells' values with new data.
```python
def replace(self, int_value, new_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| int_value | int | The integer value to be replaced. |
| new_value | System.Object | New value. Can be string, integer, double or DateTime value. |
## replace(self, place_holder, new_values, is_vertical) {#System.String-list-bool}
Replaces a cell's value with a new string array.
```python
def replace(self, place_holder, new_values, is_vertical):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | System.String | Cell placeholder |
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
## replace(self, place_holder, new_values, is_vertical) {#System.String-list-bool}
Replaces cells' values with an integer array.
```python
def replace(self, place_holder, new_values, is_vertical):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | System.String | Cell placeholder |
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
## replace(self, place_holder, new_values, is_vertical) {#System.String-list-bool}
Replaces cells' values with a double array.
```python
def replace(self, place_holder, new_values, is_vertical):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | System.String | Cell placeholder |
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
## replace(self, place_holder, new_value, options) {#System.String-System.String-aspose.cells.ReplaceOptions}
Replaces a cell's value with a new string.
```python
def replace(self, place_holder, new_value, options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| place_holder | System.String | Cell placeholder |
| new_value | System.String | String value to replace |
| options | aspose.cells.ReplaceOptions | The replace options |
### See Also
* module [`aspose.cells`](../../)
* class [`Workbook`](/cells/python-net/aspose.cells/workbook)
