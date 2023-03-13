---
title: import_csv方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 630
url: /zh/python-net/aspose.cells/cells/import_csv/
is_root: false
---
##  import_csv(file_name, options, first_row, first_column) {#str-TxtLoadOptions-int-int}
将 CSV 文件导入单元格。



```python
def import_csv(self, file_name, options, first_row, first_column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| file_name | str | CSV 文件名。|
| options | [TxtLoadOptions](/cells/zh/python-net/aspose.cells/txtloadoptions) |读取文本文件的加载选项|
| first_row | int |要导入的第一个单元格的行号。|
| first_column | int |要导入的第一个单元格的列号。|


##  import_csv(stream, options, first_row, first_column) {#io.RawIOBase-TxtLoadOptions-int-int}
将 CSV 文件导入单元格。



```python
def import_csv(self, stream, options, first_row, first_column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| stream | io.RawIOBase |CSV 文件流。|
| options | [TxtLoadOptions](/cells/zh/python-net/aspose.cells/txtloadoptions) |读取文本文件的加载选项|
| first_row | int |要导入的第一个单元格的行号。|
| first_column | int |要导入的第一个单元格的列号。|


##  import_csv(file_name, splitter, convert_numeric_data, first_row, first_column) {#str-str-bool-int-int}
将 CSV 文件导入单元格。



```python
def import_csv(self, file_name, splitter, convert_numeric_data, first_row, first_column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| file_name | str | CSV 文件名。|
| splitter | str |分离器|
| convert_numeric_data | bool |文本文件中的字符串是否转换为数字数据。|
| first_row | int |要导入的第一个单元格的行号。|
| first_column | int |要导入的第一个单元格的列号。|


##  import_csv(stream, splitter, convert_numeric_data, first_row, first_column) {#io.RawIOBase-str-bool-int-int}
将 CSV 文件导入单元格。



```python
def import_csv(self, stream, splitter, convert_numeric_data, first_row, first_column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| stream | io.RawIOBase |CSV 文件流。|
| splitter | str |分离器|
| convert_numeric_data | bool |文本文件中的字符串是否转换为数字数据。|
| first_row | int |要导入的第一个单元格的行号。|
| first_column | int |要导入的第一个单元格的列号。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cells](/cells/zh/python-net/aspose.cells/cells)
