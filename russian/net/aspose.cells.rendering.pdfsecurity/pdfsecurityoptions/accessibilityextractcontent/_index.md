---
title: "PdfSecurityOptions.AccessibilityExtractContent"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PdfSecurityOptions. Указывает, разрешено ли извлекать текст и графику в поддержку доступности для пользователей с ограниченными возможностями или для других целей."
type: docs
url: /ru/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/accessibilityextractcontent/
---
## PdfSecurityOptions.AccessibilityExtractContent property

Указывает, разрешено ли извлекать текст и графику (в целях обеспечения доступности для пользователей с ограниченными возможностями или для других целей).

```csharp
public bool AccessibilityExtractContent { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAccessibilityExtractContentDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test Accessibility Extract Content";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.AccessibilityExtractContent = true;
            pdfSecurityOptions.ExtractContentPermission = false;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("AccessibilityExtractContentDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### См. также

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


