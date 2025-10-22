##set_array_formula method
## set_array_formula(self, array_formula, row_number, column_number) {#System.String-int-int}
Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells.
```python
def set_array_formula(self, array_formula, row_number, column_number):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | System.String | Array formula. |
| row_number | int | Number of rows to populate result of the array formula. |
| column_number | int | Number of columns to populate result of the array formula. |
## set_array_formula(self, array_formula, row_number, column_number, options) {#System.String-int-int-aspose.cells.FormulaParseOptions}
Sets an array formula to a range of cells.
```python
def set_array_formula(self, array_formula, row_number, column_number, options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | System.String | Array formula. |
| row_number | int | Number of rows to populate result of the array formula. |
| column_number | int | Number of columns to populate result of the array formula. |
| options | aspose.cells.FormulaParseOptions | Options for parsing the formula. |
## set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local) {#System.String-int-int-bool-bool}
Sets an array formula to a range of cells.
```python
def set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | System.String | Array formula. |
| row_number | int | Number of rows to populate result of the array formula. |
| column_number | int | Number of columns to populate result of the array formula. |
| is_r1c1 | bool | whether the formula is R1C1 formula |
| is_local | bool | whether the formula is locale formatted |
### Remarks
NOTE: This class is now obsolete. Instead,
please use Cell.SetArrayFormula(string,int,int,FormulaParseOptions).
This property will be removed 12 months later since December 2019.
Aspose apologizes for any inconvenience you may have experienced.
## set_array_formula(self, array_formula, row_number, column_number, options, values) {#System.String-int-int-aspose.cells.FormulaParseOptions-list}
Sets an array formula to a range of cells.
```python
def set_array_formula(self, array_formula, row_number, column_number, options, values):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | System.String | Array formula. |
| row_number | int | Number of rows to populate result of the array formula. |
| column_number | int | Number of columns to populate result of the array formula. |
| options | aspose.cells.FormulaParseOptions | Options for parsing the formula. |
| values | list | values for those cells with given array formula |
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
