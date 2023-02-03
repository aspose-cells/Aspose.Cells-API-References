---
title: register_add_in_function method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 170
url: /python-net/aspose.cells/worksheetcollection/register_add_in_function/
is_root: false
---

## register_add_in_function(id, function_name) {#int-str}

Adds addin function into the workbook


### Returns 


URL of the addin file which contains addin functions


```python
def register_add_in_function(self, id, function_name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| id | int | ID of the data which contains addin functions,<br/>can be got by the first call of [WorksheetCollection.register_add_in_function(add_in_file, function_name, lib)](/cells/python-net/aspose.cells/worksheetcollection/register_add_in_function) for the same addin file. |
| function_name | str | the addin function name |


## register_add_in_function(add_in_file, function_name, lib) {#str-str-bool}

Adds addin function into the workbook


### Returns 


ID of the data which contains given addin function


```python
def register_add_in_function(self, add_in_file, function_name, lib):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| add_in_file | str | the file contains the addin functions |
| function_name | str | the addin function name |
| lib | bool | whether the given addin file is in the directory or sub-directory of Workbook Add-In library.<br/>This flag takes effect and makes difference when given addInFile is of relative path:<br/>true denotes the path is relative to Add-In library and false denotes the path is relative to this Workbook. |



### See Also
* module [aspose.cells](../../)
* class [WorksheetCollection](/cells/python-net/aspose.cells/worksheetcollection)
