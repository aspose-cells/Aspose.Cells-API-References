---
title: Aspose::Cells::PdfSaveOptions::GetSecurityOptions method
linktitle: GetSecurityOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::GetSecurityOptions method. Set this options, when security is need in xls2pdf result in C++.'
type: docs
weight: 1200
url: /fr/cpp/aspose.cells/pdfsaveoptions/getsecurityoptions/
---
## PdfSaveOptions::GetSecurityOptions method


Set this options, when security is need in xls2pdf result.

```cpp
PdfSecurityOptions Aspose::Cells::PdfSaveOptions::GetSecurityOptions()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Le code suivant définit une impression haute résolution pour le PDF de sortie.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Aspose");

PdfSaveOptions pdfSaveOptions;
PdfSecurityOptions pdfSecurityOptions;

//définir le mot de passe du propriétaire
pdfSecurityOptions.SetOwnerPassword(u"YourOwnerPassword");

//définir le mot de passe de l’utilisateur
pdfSecurityOptions.SetUserPassword(u"YourUserPassword");

//définir la permission d’impression
pdfSecurityOptions.SetPrintPermission(true);

//définir la haute résolution pour l’impression
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
