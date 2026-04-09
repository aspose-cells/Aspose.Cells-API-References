---
title: Aspose::Cells::PdfSaveOptions::GetSecurityOptions method
linktitle: GetSecurityOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::GetSecurityOptions method. Set this options, when security is need in xls2pdf result in C++.'
type: docs
weight: 1200
url: /it/cpp/aspose.cells/pdfsaveoptions/getsecurityoptions/
---
## PdfSaveOptions::GetSecurityOptions method


Set this options, when security is need in xls2pdf result.

```cpp
PdfSecurityOptions Aspose::Cells::PdfSaveOptions::GetSecurityOptions()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Il codice seguente imposta la stampa ad alta risoluzione per il PDF di output.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Aspose");

PdfSaveOptions pdfSaveOptions;
PdfSecurityOptions pdfSecurityOptions;

//imposta password del proprietario
pdfSecurityOptions.SetOwnerPassword(u"YourOwnerPassword");

//imposta password dell'utente
pdfSecurityOptions.SetUserPassword(u"YourUserPassword");

//imposta permesso di stampa
pdfSecurityOptions.SetPrintPermission(true);

//imposta alta risoluzione per la stampa
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
