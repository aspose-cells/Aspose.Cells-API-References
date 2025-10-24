##get_instance method
## get_instance(self, collection) {#list}
Creates ICellsDataTable from given collection.
### Returns
Instance of ICellsDataTable
```python
def get_instance(self, collection):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| collection | list | the collection to build table |
## get_instance(self, vals, column_names) {#list-list}
Creates ICellsDataTable from given sequence of int values.
### Returns
Instance of ICellsDataTable
```python
def get_instance(self, vals, column_names):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| vals | list | int values to build table |
| column_names | list | Column names of the table.
## get_instance(self, vals, vertial) {#list-bool}
Creates ICellsDataTable from given sequence of int values.
### Returns
Instance of ICellsDataTable
```python
def get_instance(self, vals, vertial):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| vals | list | int values to build table |
| vertial | bool | whether build table by the int values vertiacally(true) or horizontally(false) |
## get_instance(self, vals, column_names) {#list-list}
Creates ICellsDataTable from given sequence of double values.
### Returns
Instance of ICellsDataTable
```python
def get_instance(self, vals, column_names):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| vals | list | double values to build table |
| column_names | list | Column names of the table.
## get_instance(self, vals, vertial) {#list-bool}
Creates ICellsDataTable from given sequence of double values.
### Returns
Instance of ICellsDataTable
```python
def get_instance(self, vals, vertial):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| vals | list | double values to build table |
| vertial | bool | whether build table by the double values vertiacally(true) or horizontally(false) |
## get_instance(self, vals, column_names) {#list-list}
Creates ICellsDataTable from given sequence of objects.
### Returns
Instance of ICellsDataTable
```python
def get_instance(self, vals, column_names):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| vals | list | objects to build table |
| column_names | list | Column names of the table.
## get_instance(self, vals, vertial) {#list-bool}
Creates ICellsDataTable from given sequence of objects.
### Returns
Instance of ICellsDataTable
```python
def get_instance(self, vals, vertial):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| vals | list | objects to build table |
| vertial | bool | whether build table by the objects vertiacally(true) or horizontally(false) |
## get_instance(self, collection, has_header) {#list-bool}
Creates ICellsDataTable from given collection.
### Returns
Instance of ICellsDataTable
```python
def get_instance(self, collection, has_header):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| collection | list | the collection to build table |
| has_header | bool | Indicates whether the first row is header |
## get_instance(self, vals, has_header, column_names) {#list-bool-list}
Creates ICellsDataTable from given sequence of objects.
### Returns
Instance of ICellsDataTable
```python
def get_instance(self, vals, has_header, column_names):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| vals | list | objects to build table |
| has_header | bool | Indicates whether the first row is header row. |
| column_names | list | Column names of the table.
### See Also
* module [`aspose.cells`](../../)
* class [`CellsDataTableFactory`](/cells/python-net/aspose.cells/cellsdatatablefactory)
* class [`ICellsDataTable`](/cells/python-net/aspose.cells/icellsdatatable)
