---
title: Aspose::Cells::PdfSaveOptions::GetSecurityOptions method
linktitle: GetSecurityOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::GetSecurityOptions method. Set this options, when security is need in xls2pdf result in C++.'
type: docs
weight: 1200
url: /zh/cpp/aspose.cells/pdfsaveoptions/getsecurityoptions/
---
## PdfSaveOptions::GetSecurityOptions method


Set this options, when security is need in xls2pdf result.

```cpp
PdfSecurityOptions Aspose::Cells::PdfSaveOptions::GetSecurityOptions()
```


## Examples


```cpp
Aspose::Cells::Startup();
//以下代码为输出 pdf 设置高分辨率打印权限。
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Aspose");

PdfSaveOptions pdfSaveOptions;
PdfSecurityOptions pdfSecurityOptions;

//设置所有者密码
pdfSecurityOptions.SetOwnerPassword(u"YourOwnerPassword");

//设置用户密码
pdfSecurityOptions.SetUserPassword(u"YourUserPassword");

//设置打印权限
pdfSecurityOptions.SetPrintPermission(true);

//设置打印的高分辨率
pdfSecurityOptions.SetFullQualityPrintPermission(true);


if (pdfSaveOptions.GetSecurityOptions().IsNull())
{
    pdfSaveOptions.SetSecurityOptions(pdfSecurityOptions);
}

wb.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```

## See Also

* Class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* Class [PdfSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
