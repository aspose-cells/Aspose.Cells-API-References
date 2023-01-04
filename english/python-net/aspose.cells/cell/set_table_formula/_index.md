---
title: set_table_formula method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 350
url: /python-net/aspose.cells/cell/set_table_formula/
is_root: false
---

## set_table_formula(row_number, column_number, row_input_cell, column_input_cell, values) {#int-int-str-str-list}

Create two-variable data table for given range starting from this cell.



```python
def set_table_formula(self, row_number, column_number, row_input_cell, column_input_cell, values):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
| row_input_cell | str | the row input cell |
| column_input_cell | str | the column input cell |
| values | list | values for cells in table formula range |


## set_table_formula(row_number, column_number, input_cell, is_row_input, values) {#int-int-str-bool-list}

Create one-variable data table for given range starting from this cell.



```python
def set_table_formula(self, row_number, column_number, input_cell, is_row_input, values):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
| input_cell | str | the input cell |
| is_row_input | bool | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | list | values for cells in table formula range |


## set_table_formula(row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values) {#int-int-int-int-bool-list}

Create one-variable data table for given range starting from this cell.



```python
def set_table_formula(self, row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
| row_index_of_input_cell | int | row index of the input cell |
| column_index_of_input_cell | int | column index of the input cell |
| is_row_input | bool | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | list | values for cells in table formula range |


## set_table_formula(row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values) {#int-int-int-int-int-int-list}

Create two-variable data table for given range starting from this cell.



```python
def set_table_formula(self, row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
| row_index_of_row_input_cell | int | row index of the row input cell |
| column_index_of_row_input_cell | int | column index of the row input cell |
| row_index_of_column_input_cell | int | row index of the column input cell |
| column_index_of_column_input_cell | int | column index of the column input cell |
| values | list | values for cells in table formula range |



### See Also
* module [aspose.cells](../../)
* class [Cell](/cells/python-net/aspose.cells/cell)
