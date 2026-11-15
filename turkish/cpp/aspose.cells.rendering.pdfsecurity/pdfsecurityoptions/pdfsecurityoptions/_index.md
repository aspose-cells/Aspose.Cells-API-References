---
title: Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions constructor
linktitle: PdfSecurityOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions constructor. The constructor of PdfSecurityOptions in C++.'
type: docs
weight: 100
url: /tr/cpp/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/pdfsecurityoptions/
---
## PdfSecurityOptions::PdfSecurityOptions() constructor


The constructor of [PdfSecurityOptions](../).

```cpp
Aspose::Cells::Rendering::PdfSecurity::PdfSecurityOptions::PdfSecurityOptions()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Aşağıdaki kod, çıktı pdf için yüksek çözünürlüklü yazdırma iznini ayarlar.
Workbook wb;
wb.GetWorksheets().Get(0).GetCells().Get(u"A1").PutValue(u"Aspose");

PdfSaveOptions pdfSaveOptions;
PdfSecurityOptions pdfSecurityOptions;

//sahip şifresini ayarla
pdfSecurityOptions.SetOwnerPassword(u"YourOwnerPassword");

//kullanıcı şifresini ayarla
pdfSecurityOptions.SetUserPassword(u"YourUserPassword");

//baskı iznini ayarla
pdfSecurityOptions.SetPrintPermission(true);

//baskı için yüksek çözünürlüğü ayarla
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
