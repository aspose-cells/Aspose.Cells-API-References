---
title: import_custom_objects方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 640
url: /zh/python-net/aspose.cells/cells/import_custom_objects/
is_root: false
---
##  import_custom_objects(list, first_row, first_column, options) {#list-int-int-ImportTableOptions}
导入自定义对象。


### 返回

导入的总行数。


```python
def import_custom_objects(self, list, first_row, first_column, options):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| list | list |自定义对象|
| first_row | int |要导入的第一个单元格的行号。|
| first_column | int |要导入的第一个单元格的列号。|
| options | [ImportTableOptions](/cells/zh/python-net/aspose.cells/importtableoptions) |导入选项。|
### 评论

自定义对象应该是同一类型。

##  import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number) {#list-list-bool-int-int-int-bool-str-bool}

导入自定义对象。


### 返回

导入的总行数。


```python
def import_custom_objects(self, list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| list | list |自定义对象|
| property_names | list |属性名称。如果为空，我们将导入该对象的所有属性。|
| is_property_name_shown | bool |指示是否将属性名称导入到第一行。|
| first_row | int |要导入的第一个单元格的行号。|
| first_column | int |要导入的第一个单元格的列号。|
| row_number | int |要导入的行数。|
| insert_rows | bool |指示是否添加额外的行以适合数据。|
| date_format_string | str |单元格的日期格式字符串。|
| convert_string_to_number | bool |指示此方法是否将尝试将字符串转换为数字。|
### 评论

自定义对象应该是同一类型。


### 也可以看看

* 模块 [aspose.cells](../../)
* 类 [Cells](/cells/zh/python-net/aspose.cells/cells)
