##put_value method
## put_value(self, bool_value) {#bool}
Puts a boolean value into the cell.
```python
def put_value(self, bool_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| bool_value | bool |  |
## put_value(self, int_value) {#int}
Puts an integer value into the cell.
```python
def put_value(self, int_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| int_value | int | Input value |
## put_value(self, double_value) {#float}
Puts a double value into the cell.
```python
def put_value(self, double_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| double_value | float | Input value |
## put_value(self, string_value) {#System.String}
Puts a string value into the cell.
```python
def put_value(self, string_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| string_value | System.String | Input value |
## put_value(self, date_time) {#System.DateTime}
Puts a DateTime value into the cell.
```python
def put_value(self, date_time):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| date_time | System.DateTime | Input value |
### Remarks
Setting a DateTime value for a cell dose not means the cell will be formatted as date time automatically.
DateTime value was maintained as numeric value in the data model of both ms excel and Aspose.Cells.
Whether the numeric value will be taken as the numeric value itself or date time
depends on the number format applied on this cell. If this cell has not been formatted as date time,
it will be displayed as a numeric value even though what you input is DateTime.
### Example
This example shows how to set DateTime value to a cell and make it be displayed as date time.
```python
from aspose.cells import Workbook
from datetime import datetime
excel = Workbook()
cells = excel.worksheets[0].cells
# Put date time into a cell
cell = cells.get(0, 0)
cell.put_value(datetime(2023, 5, 15))
style = cell.get_style(False)
style.number = 14
cell.set_style(style)
```
## put_value(self, object_value) {#System.Object}
Puts an object value into the cell.
```python
def put_value(self, object_value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| object_value | System.Object | input value |
## put_value(self, string_value, is_converted) {#System.String-bool}
Puts a string value into the cell and converts the value to other data type if appropriate.
```python
def put_value(self, string_value, is_converted):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| string_value | System.String | Input value |
| is_converted | bool | True: converted to other data type if appropriate. |
## put_value(self, string_value, is_converted, set_style) {#System.String-bool-bool}
Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.
```python
def put_value(self, string_value, is_converted, set_style):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| string_value | System.String | Input value |
| is_converted | bool | True: converted to other data type if appropriate. |
| set_style | bool | True: set the number format to cell's style when converting to other data type |
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
