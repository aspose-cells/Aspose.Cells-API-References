---
title: set_table_formula方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 350
url: /zh/python-net/aspose.cells/cell/set_table_formula/
is_root: false
---
##  set_table_formula(row_number, column_number, row_input_cell, column_input_cell, values) {#int-int-str-str-list}
从此单元格开始为给定范围创建双变量数据表。



```python
def set_table_formula(self, row_number, column_number, row_input_cell, column_input_cell, values):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row_number | int |填充公式的行数。|
| column_number | int |填充公式的列数。|
| row_input_cell | str |行输入单元格|
| column_input_cell | str |列输入单元格|
| values | list |表格公式范围内单元格的值|


##  set_table_formula(row_number, column_number, input_cell, is_row_input, values) {#int-int-str-bool-list}
从此单元格开始为给定范围创建单变量数据表。



```python
def set_table_formula(self, row_number, column_number, input_cell, is_row_input, values):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row_number | int |填充公式的行数。|
| column_number | int |填充公式的列数。|
| input_cell | str |输入单元格|
| is_row_input | bool |指示输入单元格是行输入单元格 (true) 还是列输入单元格 (false)。|
| values | list |表格公式范围内单元格的值|


##  set_table_formula(row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values) {#int-int-int-int-bool-list}
从此单元格开始为给定范围创建单变量数据表。



```python
def set_table_formula(self, row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row_number | int |填充公式的行数。|
| column_number | int |填充公式的列数。|
| row_index_of_input_cell | int |输入单元格的行索引|
| column_index_of_input_cell | int |输入单元格的列索引|
| is_row_input | bool |指示输入单元格是行输入单元格 (true) 还是列输入单元格 (false)。|
| values | list |表格公式范围内单元格的值|


##  set_table_formula(row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values) {#int-int-int-int-int-int-list}
从此单元格开始为给定范围创建双变量数据表。



```python
def set_table_formula(self, row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row_number | int |填充公式的行数。|
| column_number | int |填充公式的列数。|
| row_index_of_row_input_cell | int |行输入单元格的行索引|
| column_index_of_row_input_cell | int |行输入单元格的列索引|
| row_index_of_column_input_cell | int |列输入单元格的行索引|
| column_index_of_column_input_cell | int |列输入单元格的列索引|
| values | list |表格公式范围内单元格的值|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
