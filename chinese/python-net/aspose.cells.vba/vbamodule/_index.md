---
title: VbaModule类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 10
url: /zh/python-net/aspose.cells.vba/vbamodule/
is_root: false
---
##  VbaModule类
表示 VBA 项目中的模块。



VbaModule 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [name](/cells/zh/python-net/aspose.cells.vba/vbamodule/name) |获取和设置模块的名称。|
| [type](/cells/zh/python-net/aspose.cells.vba/vbamodule/type) |获取模块类型。|
| [codes](/cells/zh/python-net/aspose.cells.vba/vbamodule/codes) |获取和设置模块的代码。|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.vba import VbaModuleType

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add a new module.
index = vbaProject.modules.add(VbaModuleType.CLASS, "test")
#  Get vba module
vbaModule = vbaProject.modules[index]
#  Set codes
vbaModule.codes = "Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub"
# Saving the Excel file
workbook.save("book1.xlsm")

```

### 也可以看看
* 模块 [aspose.cells.vba](..)
