---
title: Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions constructor
linktitle: PdfSecurityOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions constructor. The constructor of PdfSecurityOptions in C++.'
type: docs
weight: 100
url: /it/cpp/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/pdfsecurityoptions/
---
## PdfSecurityOptions::PdfSecurityOptions() constructor


The constructor of [PdfSecurityOptions](../).

```cpp
Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Il codice seguente imposta l'autorizzazione di stampa ad alta risoluzione per il PDF di output.
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


pdfSaveOptions.SetSecurityOptions(pdfSecurityOptions);

wb.Save(u"output.pdf", pdfSaveOptions);
Aspose::Cells::Cleanup();
```

## See Also

* Class [PdfSecurityOptions](../)
* Namespace [Aspose::Cells::Rendering::PdfSecurity](../../)
* Library [Aspose.Cells for C++](../../../)
## PdfSecurityOptions::PdfSecurityOptions(PdfSecurityOptions_Impl*) constructor


Constructs from an implementation object.

```cpp
Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions(PdfSecurityOptions_Impl *impl)
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PdfSecurityOptions](../)
* Namespace [Aspose::Cells::Rendering::PdfSecurity](../../)
* Library [Aspose.Cells for C++](../../../)
## PdfSecurityOptions::PdfSecurityOptions(const PdfSecurityOptions\&) constructor


Copy constructor.

```cpp
Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions(const PdfSecurityOptions &src)
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [PdfSecurityOptions](../)
* Class [PdfSecurityOptions](../)
* Namespace [Aspose::Cells::Rendering::PdfSecurity](../../)
* Library [Aspose.Cells for C++](../../../)
