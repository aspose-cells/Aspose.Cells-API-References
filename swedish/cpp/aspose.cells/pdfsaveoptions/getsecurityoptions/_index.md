---
title: Aspose::Cells::PdfSaveOptions::GetSecurityOptions method
linktitle: GetSecurityOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::GetSecurityOptions method. Set this options, when security is need in xls2pdf result in C++.'
type: docs
weight: 1200
url: /sv/cpp/aspose.cells/pdfsaveoptions/getsecurityoptions/
---
## PdfSaveOptions::GetSecurityOptions method


Set this options, when security is need in xls2pdf result.

```cpp
PdfSecurityOptions Aspose::Cells::PdfSaveOptions::GetSecurityOptions()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Följande kod ställer in högupplöst utskriftsbehörighet för den genererade pdf-filen.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Aspose");

PdfSaveOptions pdfSaveOptions;
PdfSecurityOptions pdfSecurityOptions;

//ange ägarlösenord
pdfSecurityOptions.SetOwnerPassword(u"YourOwnerPassword");

//ange användarlösenord
pdfSecurityOptions.SetUserPassword(u"YourUserPassword");

//ange utskriftsbehörighet
pdfSecurityOptions.SetPrintPermission(true);

//ange hög upplösning för utskrift
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
