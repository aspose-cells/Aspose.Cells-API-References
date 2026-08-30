---
title: Aspose::Cells::PdfSaveOptions::SetSecurityOptions method
linktitle: SetSecurityOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::PdfSaveOptions::SetSecurityOptions method. Set this options, when security is need in xls2pdf result in C++.'
type: docs
weight: 1300
url: /es/cpp/aspose.cells/pdfsaveoptions/setsecurityoptions/
---
## PdfSaveOptions::SetSecurityOptions method


Set this options, when security is need in xls2pdf result.

```cpp
void Aspose::Cells::PdfSaveOptions::SetSecurityOptions(const PdfSecurityOptions &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//El siguiente código establece permiso de impresión de alta resolución para el pdf de salida.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Aspose");

PdfSaveOptions pdfSaveOptions;
PdfSecurityOptions pdfSecurityOptions;

//establecer contraseña de propietario
pdfSecurityOptions.SetOwnerPassword(u"YourOwnerPassword");

//establecer contraseña de usuario
pdfSecurityOptions.SetUserPassword(u"YourUserPassword");

//establecer permiso de impresión
pdfSecurityOptions.SetPrintPermission(true);

//establecer alta resolución para la impresión
pdfSecurityOptions.SetFullQualityPrintPermission(true);


if (pdfSaveOptions.GetSecurityOptions().IsNull())
{
    pdfSaveOptions.SetSecurityOptions(pdfSecurityOptions);
}

wb.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../vector/)
* Class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* Class [PdfSaveOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
