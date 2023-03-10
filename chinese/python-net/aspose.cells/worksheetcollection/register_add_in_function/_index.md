---
title: register_add_in_function方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 170
url: /zh/python-net/aspose.cells/worksheetcollection/register_add_in_function/
is_root: false
---
##  register_add_in_function(id, function_name) {#int-str}
将插件功能添加到工作簿中


### 返回

包含插件函数的插件文件的 URL


```python
def register_add_in_function(self, id, function_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| id | int |包含插件函数的数据的 ID，<br/>可以通过第一次调用 [WorksheetCollection.register_add_in_function(add_in_file, function_name, lib)](/cells/zh/python-net/aspose.cells/worksheetcollection/register_add_in_function) 获取相同的插件文件。|
| function_name | str |插件函数名称|


##  register_add_in_function(add_in_file, function_name, lib) {#str-str-bool}
将插件功能添加到工作簿中


### 返回

包含给定插件函数的数据的 ID


```python
def register_add_in_function(self, add_in_file, function_name, lib):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| add_in_file | str |该文件包含插件函数|
| function_name | str |插件函数名称|
| lib | bool |给定的加载项文件是否在工作簿加载项库的目录或子目录中。<br/>当给定的 addInFile 是相对路径时，此标志生效并有所不同：<br/> true 表示路径是相对于 Add-In 库的，false 表示路径是相对于此工作簿的。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [WorksheetCollection](/cells/zh/python-net/aspose.cells/worksheetcollection)
