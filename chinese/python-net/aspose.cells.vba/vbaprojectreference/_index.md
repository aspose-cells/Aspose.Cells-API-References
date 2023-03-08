---
title: VbaProjectReference类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells.vba/vbaprojectreference/
is_root: false
---
##  VbaProjectReference类
代表VBA工程的引用。



VbaProjectReference 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [type](/cells/zh/python-net/aspose.cells.vba/vbaprojectreference/type) |获取此引用的类型。|
| [name](/cells/zh/python-net/aspose.cells.vba/vbaprojectreference/name) |获取和设置引用的名称。|
| [libid](/cells/zh/python-net/aspose.cells.vba/vbaprojectreference/libid) |获取和设置引用的 Libid。|
| [twiddledlibid](/cells/zh/python-net/aspose.cells.vba/vbaprojectreference/twiddledlibid) |获取和设置引用的 twiddled Libid。|
| [extended_libid](/cells/zh/python-net/aspose.cells.vba/vbaprojectreference/extended_libid) |获取和设置引用的扩展 Libid。|
| [relative_libid](/cells/zh/python-net/aspose.cells.vba/vbaprojectreference/relative_libid) |使用相对路径获取和设置引用的 VBA 项目的标识符。|


### 方法
|方法|描述|
| :- | :- |
| [copy(source)](/cells/zh/python-net/aspose.cells.vba/vbaprojectreference/copy/#VbaProjectReference) |  |



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add vba project reference
vbaProject.references.add_registered_reference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation")
# Saving the Excel file
workbook.save("book1.xlsm")

```

### 也可以看看
* 模块 [aspose.cells.vba](..)
