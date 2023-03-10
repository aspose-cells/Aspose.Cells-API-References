---
title: VbaProject类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells.vba/vbaproject/
is_root: false
---
## VbaProject类
表示 VBA 项目。



VbaProject 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [is_valid_signed](/cells/zh/python-net/aspose.cells.vba/vbaproject/is_valid_signed) |指示 VBA 项目的签名是否有效。|
| [cert_raw_data](/cells/zh/python-net/aspose.cells.vba/vbaproject/cert_raw_data) |如果此 VBA 项目已签名，则获取证书原始数据。|
| [name](/cells/zh/python-net/aspose.cells.vba/vbaproject/name) |获取和设置 VBA 项目的名称。|
| [is_signed](/cells/zh/python-net/aspose.cells.vba/vbaproject/is_signed) |指示 VBAcode 是否已签名。|
| [is_protected](/cells/zh/python-net/aspose.cells.vba/vbaproject/is_protected) |指示此 VBA 项目是否受保护。|
| [islocked_for_viewing](/cells/zh/python-net/aspose.cells.vba/vbaproject/islocked_for_viewing) |指示此 VBA 项目是否已锁定以供查看。|
| [modules](/cells/zh/python-net/aspose.cells.vba/vbaproject/modules) |获取所有 [VbaModule](/cells/zh/python-net/aspose.cells.vba/vbamodule) 对象。|
| [references](/cells/zh/python-net/aspose.cells.vba/vbaproject/references) |获取 VBA 项目的所有引用。|


### 方法
|方法|描述|
| :- | :- |
| [sign(digital_signature)](/cells/zh/python-net/aspose.cells.vba/vbaproject/sign/#aspose.cells.digitalsignatures.DigitalSignature) |通过 DigitalSignature 签署此 VBA 项目|
| [protect(islocked_for_viewing, password)](/cells/zh/python-net/aspose.cells.vba/vbaproject/protect/#bool-str) |保护或取消保护此 VBA 项目。|
| [copy(source)](/cells/zh/python-net/aspose.cells.vba/vbaproject/copy/#VbaProject) |从其他文件复制 VBA 项目。|
| [validate_password(password)](/cells/zh/python-net/aspose.cells.vba/vbaproject/validate_password/#str) |验证保护密码。|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
# Saving the Excel file
workbook.save("book1.xlsm")

```

### 也可以看看
* 模块 [aspose.cells.vba](..)
* 类 [VbaModule](/cells/zh/python-net/aspose.cells.vba/vbamodule)
