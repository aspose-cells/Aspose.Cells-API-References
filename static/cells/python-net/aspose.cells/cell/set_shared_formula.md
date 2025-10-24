##set_shared_formula method
## set_shared_formula(self, shared_formula, row_number, column_number) {#System.String-int-int}
Sets shared formulas to a range of cells.
```python
def set_shared_formula(self, shared_formula, row_number, column_number):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| shared_formula | System.String | Shared formula. |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
### Remarks
## set_shared_formula(self, shared_formula, row_number, column_number, options) {#System.String-int-int-aspose.cells.FormulaParseOptions}
Sets shared formulas to a range of cells.
```python
def set_shared_formula(self, shared_formula, row_number, column_number, options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| shared_formula | System.String | Shared formula. |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
| options | aspose.cells.FormulaParseOptions | Options for parsing the formula. |
## set_shared_formula(self, shared_formula, row_number, column_number, is_r1c1, is_local) {#System.String-int-int-bool-bool}
Sets a formula to a range of cells.
```python
def set_shared_formula(self, shared_formula, row_number, column_number, is_r1c1, is_local):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| shared_formula | System.String | Shared formula. |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
| is_r1c1 | bool | whether the formula is R1C1 formula |
| is_local | bool | whether the formula is locale formatted |
### Remarks
NOTE: This class is now obsolete. Instead,
please use Cell.SetSharedFormula(string,int,int,FormulaParseOptions).
This property will be removed 12 months later since December 2019.
Aspose apologizes for any inconvenience you may have experienced.
## set_shared_formula(self, shared_formula, row_number, column_number, options, values) {#System.String-int-int-aspose.cells.FormulaParseOptions-list}
Sets shared formulas to a range of cells.
```python
def set_shared_formula(self, shared_formula, row_number, column_number, options, values):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| shared_formula | System.String | Shared formula. |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
| options | aspose.cells.FormulaParseOptions | Options for parsing the formula. |
| values | list | values for those cells with given shared formula |
### See Also
* module [`aspose.cells`](../../)
* class [`Cell`](/cells/python-net/aspose.cells/cell)
