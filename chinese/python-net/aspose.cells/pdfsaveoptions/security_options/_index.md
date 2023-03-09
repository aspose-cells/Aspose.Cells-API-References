---
title: security_options 属性
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 390
url: /zh/python-net/aspose.cells/pdfsaveoptions/security_options/
is_root: false
---
## security_options 属性

在 xls2pdf 结果中需要安全性时设置此选项。

### 例子

以下代码为输出 pdf 设置高分辨率打印权限。

```python
from aspose.cells import PdfSaveOptions, Workbook
from aspose.cells.rendering.pdfsecurity import PdfSecurityOptions

wb = Workbook()
wb.worksheets[0].cells.get("A1").value = "Aspose"
pdfSaveOptions = PdfSaveOptions()
pdfSecurityOptions = PdfSecurityOptions()
# set owner password
pdfSecurityOptions.owner_password = "YourOwnerPassword"
# set user password
pdfSecurityOptions.user_password = "YourUserPassword"
# set print permisson
pdfSecurityOptions.print_permission = True
# set high resolution for print
pdfSecurityOptions.full_quality_print_permission = True
pdfSaveOptions.security_options = pdfSecurityOptions
wb.save("output.pdf", pdfSaveOptions)

```
### 定义：
```python
@property
def security_options(self):
    ...
@security_options.setter
def security_options(self, value):
    ...
```

### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [PdfSaveOptions](/cells/zh/python-net/aspose.cells/pdfsaveoptions)
* 类 [PdfSecurityOptions](/cells/zh/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
