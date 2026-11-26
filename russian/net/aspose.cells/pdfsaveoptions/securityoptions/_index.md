---
title: "PdfSaveOptions.SecurityOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSaveOptions. Установите эти параметры, когда в результате xls2pdf требуется безопасность"
type: docs
url: /ru/net/aspose.cells/pdfsaveoptions/securityoptions/
---
## PdfSaveOptions.SecurityOptions property

Установите эти параметры, когда в результате xls2pdf требуется безопасность.

```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertySecurityOptionsDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Добавьте примерные данные
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF Demo";
            
            // Создайте параметры сохранения PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Настроить параметры безопасности
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;
            securityOptions.ExtractContentPermission = false;
            
            // Назначить параметры безопасности параметрам сохранения
            saveOptions.SecurityOptions = securityOptions;
            
            // Сохранить PDF с настройками безопасности
            workbook.Save("SecuredDocument.pdf", saveOptions);
            
            Console.WriteLine("PDF with security options created successfully.");
        }
    }
}
```

### См. также

* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


