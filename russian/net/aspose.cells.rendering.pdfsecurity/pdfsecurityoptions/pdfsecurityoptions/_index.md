---
title: PdfSecurityOptions
second_title: Справочник по Aspose.Cells для .NET API
description: Конструктор PdfSecurityOptions
type: docs
weight: 10
url: /ru/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/pdfsecurityoptions/
---
## PdfSecurityOptions constructor

Конструктор PdfSecurityOptions

```csharp
public PdfSecurityOptions()
```

### Примеры

Следующий код устанавливает разрешение на печать с высоким разрешением для выходного pdf.

```csharp
Workbook wb = new Workbook();
wb.Worksheets[0].Cells["A1"].Value = "Aspose";

PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();


PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

//установить пароль владельца
pdfSecurityOptions.OwnerPassword = "YourOwnerPassword";

//установить пароль пользователя
pdfSecurityOptions.UserPassword = "YourUserPassword";

//устанавливаем разрешение на печать
pdfSecurityOptions.PrintPermission = true;

//устанавливаем высокое разрешение для печати
pdfSecurityOptions.FullQualityPrintPermission = true;


pdfSaveOptions.SecurityOptions = pdfSecurityOptions;

wb.Save("output.pdf", pdfSaveOptions);
```

### Смотрите также

* class [PdfSecurityOptions](../../pdfsecurityoptions)
* пространство имен [Aspose.Cells.Rendering.PdfSecurity](../../pdfsecurityoptions)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
