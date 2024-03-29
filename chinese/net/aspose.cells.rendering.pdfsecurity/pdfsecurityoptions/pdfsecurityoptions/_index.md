---
title: PdfSecurityOptions
second_title: Aspose.Cells for .NET API 参考
description: PdfSecurityOptions 的构造函数
type: docs
weight: 10
url: /zh/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/pdfsecurityoptions/
---
## PdfSecurityOptions constructor

PdfSecurityOptions 的构造函数

```csharp
public PdfSecurityOptions()
```

### 例子

以下代码设置输出pdf的高分辨率打印权限。

```csharp
Workbook wb = new Workbook();
wb.Worksheets[0].Cells["A1"].Value = "Aspose";

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();


PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

//设置所有者密码
pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";

//设置用户密码
pdfSecurityOptions.UserPassword = "YourUserPassword";

//设置打印权限
pdfSecurityOptions.PrintPermission = true;

//设置打印的高分辨率
pdfSecurityOptions.FullQualityPrintPermission = true;


pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

wb.Save("output.pdf", pdfSaveOptions);
```

### 也可以看看

* class [PdfSecurityOptions](../../pdfsecurityoptions)
* 命名空间 [Aspose.Cells.Rendering.PdfSecurity](../../pdfsecurityoptions)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
