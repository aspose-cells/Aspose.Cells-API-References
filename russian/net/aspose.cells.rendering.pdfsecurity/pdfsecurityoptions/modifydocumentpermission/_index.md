---
title: "PdfSecurityOptions.ModifyDocumentPermission"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSecurityOptions. Указывает, разрешено ли изменять содержимое документа операциями, отличными от контролируемых AnnotationsPermission, FillFormsPermission и AssembleDocumentPermission."
type: docs
url: /ru/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/
---
## PdfSecurityOptions.ModifyDocumentPermission property

Указывает, разрешено ли изменять содержимое документа операциями, отличными от контролируемых [`AnnotationsPermission`](../annotationspermission/), [`FillFormsPermission`](../fillformspermission/) и [`AssembleDocumentPermission`](../assembledocumentpermission/).

```csharp
public bool ModifyDocumentPermission { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyModifyDocumentPermissionDemo
    {
        public static void Run()
        {
            // Создать новую книгу с примерными данными.
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            // Настройте параметры сохранения PDF с параметрами безопасности
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Установите пароли и разрешения
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.ModifyDocumentPermission = false; // Core property demonstration
            securityOptions.PrintPermission = true;

            // Применить параметры безопасности и сохранить
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredDocument.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ModifyDocumentPermission set to false");
        }
    }
}
```

### См. также

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


