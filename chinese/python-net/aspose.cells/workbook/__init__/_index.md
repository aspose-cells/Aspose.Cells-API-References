---
title: Workbook 构造函数
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 10
url: /zh/python-net/aspose.cells/workbook/__init__/
is_root: false
---
##  Workbook() {#}
初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例。



```python
def __init__(self):
    ...
```


### 评论

默认文件格式类型是 Xlsx。要创建其他格式文件类型，请使用 Workbook(FileFormatType)。
### 例子


以下代码显示如何使用 Workbook 构造函数创建和初始化该类的新实例。

```python
from aspose.cells import Workbook

workbook = Workbook()

```


##  Workbook(file_format_type) {#FileFormatType}
初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例。



```python
def __init__(self, file_format_type):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| file_format_type | [FileFormatType](/cells/zh/python-net/aspose.cells/fileformattype) |新的文件格式。|
### 评论

默认文件格式类型为 Excel97To2003。
### 例子


以下代码显示如何使用 Workbook 构造函数创建和初始化该类的新实例。

```python
from aspose.cells import FileFormatType, Workbook

workbook = Workbook(FileFormatType.XLSX)

```


##  Workbook(file) {#str}
初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例并打开一个文件。



```python
def __init__(self, file):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| file | str |文件名。|


##  Workbook(stream) {#io.RawIOBase}
初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例并打开流。



```python
def __init__(self, stream):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| stream | io.RawIOBase |流。|


##  Workbook(file, load_options) {#str-LoadOptions}
初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例并打开一个文件。



```python
def __init__(self, file, load_options):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| file | str |文件名。|
| load_options | [LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions) |加载选项|


##  Workbook(stream, load_options) {#io.RawIOBase-LoadOptions}
初始化 [Workbook](/cells/zh/python-net/aspose.cells/workbook) 类的新实例并打开流。



```python
def __init__(self, stream, load_options):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| stream | io.RawIOBase |流。|
| load_options | [LoadOptions](/cells/zh/python-net/aspose.cells/loadoptions) |加载选项|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Workbook](/cells/zh/python-net/aspose.cells/workbook)
