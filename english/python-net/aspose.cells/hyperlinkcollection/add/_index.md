---
title: add method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/hyperlinkcollection/add/
is_root: false
---

## add(cell_name, total_rows, total_columns, address) {#str-int-int-str}

Adds a hyperlink to a specified cell or a range of cells.


### Returns 


[Hyperlink](/cells/python-net/aspose.cells/hyperlink) object index.


```python
def add(self, cell_name, total_rows, total_columns, address):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| cell_name | str | Cell name. |
| total_rows | int | Number of rows in this hyperlink range. |
| total_columns | int | Number of columns of this hyperlink range. |
| address | str | Address of the hyperlink. |


## add(first_row, first_column, total_rows, total_columns, address) {#int-int-int-int-str}

Adds a hyperlink to a specified cell or a range of cells.


### Returns 


[Hyperlink](/cells/python-net/aspose.cells/hyperlink) object index.


```python
def add(self, first_row, first_column, total_rows, total_columns, address):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| first_row | int | First row of the hyperlink range. |
| first_column | int | First column of the hyperlink range. |
| total_rows | int | Number of rows in this hyperlink range. |
| total_columns | int | Number of columns of this hyperlink range. |
| address | str | Address of the hyperlink. |

### Example 


```python
from aspose.cells import Workbook

# Instantiating a Workbook object
excel = Workbook()
worksheet = excel.worksheets[0]
worksheet.hyperlinks.add("A4", 1, 1, "http://www.aspose.com")
worksheet.hyperlinks.add("A5", 1, 1, "c:\\book1.xls")

```


## add(start_cell_name, end_cell_name, address, text_to_display, screen_tip) {#str-str-str-str-str}

Adds a hyperlink to a specified cell or a range of cells.


### Returns 


[Hyperlink](/cells/python-net/aspose.cells/hyperlink) object index.


```python
def add(self, start_cell_name, end_cell_name, address, text_to_display, screen_tip):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| start_cell_name | str | The top-left cell of the range. |
| end_cell_name | str | The bottom-right cell of the range. |
| address | str | Address of the hyperlink. |
| text_to_display | str | The text to be displayed for the specified hyperlink. |
| screen_tip | str | The screenTip text for the specified hyperlink. |



### See Also
* module [aspose.cells](../../)
* class [Hyperlink](/cells/python-net/aspose.cells/hyperlink)
* class [HyperlinkCollection](/cells/python-net/aspose.cells/hyperlinkcollection)
