---
title: "PdfSecurityOptions.FillFormsPermission"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSecurityOptions. Указывает, разрешено ли заполнять существующие интерактивные поля формы, включая поля подписи, даже если свойство ModifyDocumentPermission не установлено"
type: docs
url: /ru/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/
---
## PdfSecurityOptions.FillFormsPermission property

Указывает, разрешено ли заполнять существующие интерактивные поля формы (включая поля подписи), даже если [`ModifyDocumentPermission`](../modifydocumentpermission/) не установлен.

```csharp
public bool FillFormsPermission { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyFillFormsPermissionDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "PDF Form Example";

            // Настройте параметры сохранения PDF с параметрами безопасности
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Установите пароли и разрешения
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.FillFormsPermission = true; // Key permission being demonstrated
            securityOptions.PrintPermission = true;

            // Применить параметры безопасности и сохранить
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecureFormFillEnabled.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with form filling permission enabled.");
        }
    }
}
```

### См. также

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


