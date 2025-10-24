##group_by method
## group_by(self, interval, new_field) {#float-bool}
Automatically group the field with internal
```python
def group_by(self, interval, new_field):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| interval | float | The internal of group.
| new_field | bool | Indicates whether adding a new field to the pivottable. |
## group_by(self, custom_group_items, new_field) {#list-bool}
Custom group the field.
### Returns
False means this field could not be grouped by date time.
```python
def group_by(self, custom_group_items, new_field):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| custom_group_items | list | The custom group items. |
| new_field | bool | Indicates whether adding a new field to the pivottable |
## group_by(self, start, end, interval, new_field) {#float-float-float-bool}
Group the file by number.
### Returns
False means this field could not be grouped by date time.
```python
def group_by(self, start, end, interval, new_field):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| start | float | The start value |
| end | float | The end of value |
| interval | float | The interval |
| new_field | bool | Indicates whether adding a new field to the pivottable |
## group_by(self, start, end, groups, interval, first_as_new_field) {#System.DateTime-System.DateTime-list-float-bool}
Group the file by the date group types.
### Returns
False means this field could not be grouped by date time.
```python
def group_by(self, start, end, groups, interval, first_as_new_field):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| start | System.DateTime | The start datetime |
| end | System.DateTime | The end of datetime |
| groups | list | Group types |
| interval | float | The interval |
| first_as_new_field | bool | Indicates whether adding a new field to the pivottable.
### See Also
* module [`aspose.cells.pivot`](../../)
* class [`PivotField`](/cells/python-net/aspose.cells.pivot/pivotfield)
