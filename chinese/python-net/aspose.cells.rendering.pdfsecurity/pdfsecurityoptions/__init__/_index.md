---
title: PdfSecurityOptions 构造函数
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 10
url: /zh/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/__init__/
is_root: false
---
##  PdfSecurityOptions() {#}
PdfSecurityOptions的构造函数



```python
def __init__(self):
    ...
```



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



### 也可以看看
* 模块 [aspose.cells.rendering.pdfsecurity](../../)
* 类 [PdfSecurityOptions](/cells/zh/python-net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions)
