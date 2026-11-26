---
title: "PdfSecurityOptions.OwnerPassword"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSecurityOptions. Получает или задает пароль владельца зашифрованного PDF‑документа"
type: docs
url: /ru/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/
---
## PdfSecurityOptions.OwnerPassword property

Получает или задаёт пароль владельца зашифрованного PDF‑документа.

```csharp
public string OwnerPassword { get; set; }
```

### Примечания

Пароль владельца позволяет пользователю открыть зашифрованный PDF‑документ без каких‑либо указанных ограничений доступа.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyOwnerPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with Owner Password";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;

            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredPdfWithOwnerPassword.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with owner password protection.");
        }
    }
}
```

### См. также

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


