##add method
## add(self, source_data, dest_cell_name, table_name) {#System.String-System.String-System.String}
Adds a new PivotTable.
### Returns
The new added cache index.
```python
def add(self, source_data, dest_cell_name, table_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source_data | System.String | The data for the new PivotTable cache. |
| dest_cell_name | System.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| table_name | System.String | The name of the new PivotTable report. |
## add(self, pivot_table, dest_cell_name, table_name) {#aspose.cells.pivot.PivotTable-System.String-System.String}
Adds a new PivotTable based on another PivotTable.
### Returns
The new added PivotTable index.
```python
def add(self, pivot_table, dest_cell_name, table_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot_table | aspose.cells.pivot.PivotTable | The source pivotTable. |
| dest_cell_name | System.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| table_name | System.String | The name of the new PivotTable report. |
## add(self, source_data, dest_cell_name, table_name, use_same_source) {#System.String-System.String-System.String-bool}
Adds a new PivotTable.
### Returns
The new added cache index.
```python
def add(self, source_data, dest_cell_name, table_name, use_same_source):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source_data | System.String | The data for the new PivotTable cache. |
| dest_cell_name | System.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| table_name | System.String | The name of the new PivotTable report. |
| use_same_source | bool | Indicates whether using same data source when another existing pivot table has used this data source.
## add(self, source_data, row, column, table_name) {#System.String-int-int-System.String}
Adds a new PivotTable.
### Returns
The new added cache index.
```python
def add(self, source_data, row, column, table_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source_data | System.String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| table_name | System.String | The name of the new PivotTable report. |
## add(self, pivot_table, row, column, table_name) {#aspose.cells.pivot.PivotTable-int-int-System.String}
Adds a new PivotTable based on another PivotTable.
### Returns
The new added PivotTable index.
```python
def add(self, pivot_table, row, column, table_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| pivot_table | aspose.cells.pivot.PivotTable | The source pivotTable. |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| table_name | System.String | The name of the new PivotTable report. |
## add(self, source_data, row, column, table_name, use_same_source) {#System.String-int-int-System.String-bool}
Adds a new PivotTable.
### Returns
The new added cache index.
```python
def add(self, source_data, row, column, table_name, use_same_source):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source_data | System.String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| table_name | System.String | The name of the new PivotTable report. |
| use_same_source | bool | Indicates whether using same data source when another existing pivot table has used this data source.
## add(self, source_data, cell, table_name, use_same_source, is_xls_classic) {#System.String-System.String-System.String-bool-bool}
Adds a new PivotTable.
### Returns
The new added cache index.
```python
def add(self, source_data, cell, table_name, use_same_source, is_xls_classic):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source_data | System.String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| cell | System.String | The cell in the upper-left corner of the PivotTable report's destination range. |
| table_name | System.String | The name of the new PivotTable report. |
| use_same_source | bool | Indicates whether using same data source when another existing pivot table has used this data source.
| is_xls_classic | bool | Indicates whether add classic pivot table of Excel 97-2003. |
## add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name) {#list-bool-aspose.cells.pivot.PivotPageFields-System.String-System.String}
Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.
### Returns
The new added PivotTable index.
```python
def add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source_data | list | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| is_auto_page | bool | Whether auto create a single page field.
| page_fields | aspose.cells.pivot.PivotPageFields | The pivot page field items. |
| dest_cell_name | System.String | destCellName The name of the new PivotTable report. |
| table_name | System.String | the name of the new PivotTable report. |
## add(self, source_data, row, column, table_name, use_same_source, is_xls_classic) {#System.String-int-int-System.String-bool-bool}
Adds a new PivotTable.
### Returns
The new added cache index.
```python
def add(self, source_data, row, column, table_name, use_same_source, is_xls_classic):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source_data | System.String | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| table_name | System.String | The name of the new PivotTable report. |
| use_same_source | bool | Indicates whether using same data source when another existing pivot table has used this data source.
| is_xls_classic | bool | Indicates whether add classic pivot table of Excel 97-2003. |
## add(self, source_data, is_auto_page, page_fields, row, column, table_name) {#list-bool-aspose.cells.pivot.PivotPageFields-int-int-System.String}
Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.
### Returns
The new added PivotTable index.
```python
def add(self, source_data, is_auto_page, page_fields, row, column, table_name):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source_data | list | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| is_auto_page | bool | Whether auto create a single page field.
| page_fields | aspose.cells.pivot.PivotPageFields | The pivot page field items. |
| row | int | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | int | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| table_name | System.String | The name of the new PivotTable report. |
### See Also
* module [`aspose.cells.pivot`](../../)
* class [`PivotTableCollection`](/cells/python-net/aspose.cells.pivot/pivottablecollection)
