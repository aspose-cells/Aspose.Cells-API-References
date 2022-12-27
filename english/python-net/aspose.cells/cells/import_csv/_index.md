---
title: import_csv method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 630
url: /python-net/aspose.cells/cells/import_csv/
is_root: false
---

## import_csv(file_name, options, first_row, first_column) {#str-TxtLoadOptions-int-int}

Import a CSV file to the cells.



```python
def import_csv(self, file_name, options, first_row, first_column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_name | str | The CSV file name. |
| options | [TxtLoadOptions](/cells/python-net/aspose.cells/txtloadoptions) | The load options for reading text file |
| first_row | int | The row number of the first cell to import in. |
| first_column | int | The column number of the first cell to import in. |


## import_csv(stream, options, first_row, first_column) {#io.RawIOBase-TxtLoadOptions-int-int}

Import a CSV file to the cells.



```python
def import_csv(self, stream, options, first_row, first_column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The CSV file stream. |
| options | [TxtLoadOptions](/cells/python-net/aspose.cells/txtloadoptions) | The load options for reading text file |
| first_row | int | The row number of the first cell to import in. |
| first_column | int | The column number of the first cell to import in. |


## import_csv(file_name, splitter, convert_numeric_data, first_row, first_column) {#str-str-bool-int-int}

Import a CSV file to the cells.



```python
def import_csv(self, file_name, splitter, convert_numeric_data, first_row, first_column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| file_name | str | The CSV file name. |
| splitter | str | The splitter |
| convert_numeric_data | bool | Whether the string in text file is converted to numeric data. |
| first_row | int | The row number of the first cell to import in. |
| first_column | int | The column number of the first cell to import in. |


## import_csv(stream, splitter, convert_numeric_data, first_row, first_column) {#io.RawIOBase-str-bool-int-int}

Import a CSV file to the cells.



```python
def import_csv(self, stream, splitter, convert_numeric_data, first_row, first_column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| stream | io.RawIOBase | The CSV file stream. |
| splitter | str | The splitter |
| convert_numeric_data | bool | Whether the string in text file is converted to numeric data. |
| first_row | int | The row number of the first cell to import in. |
| first_column | int | The column number of the first cell to import in. |



### See Also
* module [aspose.cells](../../)
* class [Cells](/cells/python-net/aspose.cells/cells)
