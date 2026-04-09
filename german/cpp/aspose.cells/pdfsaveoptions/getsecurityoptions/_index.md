---
title: Aspose::Cells::PdfSaveOptions::GetSecurityOptions method
linktitle: GetSecurityOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::GetSecurityOptions method. Set this options, when security is need in xls2pdf result in C++.'
type: docs
weight: 1200
url: /de/cpp/aspose.cells/pdfsaveoptions/getsecurityoptions/
---
## PdfSaveOptions::GetSecurityOptions method


Set this options, when security is need in xls2pdf result.

```cpp
PdfSecurityOptions Aspose::Cells::PdfSaveOptions::GetSecurityOptions()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Der folgende Code setzt die hochauflösende Druckberechtigung für das Ausgabe‑PDF.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Aspose");

PdfSaveOptions pdfSaveOptions;
PdfSecurityOptions pdfSecurityOptions;

//Besitzer‑Passwort festlegen
pdfSecurityOptions.SetOwnerPassword(u"YourOwnerPassword");

//Benutzer‑Passwort festlegen
pdfSecurityOptions.SetUserPassword(u"YourUserPassword");

//Druckberechtigung festlegen
pdfSecurityOptions.SetPrintPermission(true);

//Hohe Auflösung für den Druck festlegen
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
