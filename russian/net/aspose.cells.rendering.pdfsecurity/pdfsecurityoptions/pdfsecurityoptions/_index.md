---
title: "PdfSecurityOptions.PdfSecurityOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор PdfSecurityOptions. Конструктор PdfSecurityOptions."
type: docs
url: /ru/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/pdfsecurityoptions/
---
## PdfSecurityOptions constructor

Конструктор класса PdfSecurityOptions

```csharp
public PdfSecurityOptions()
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsMethodCtorDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            wb.Worksheets[0].Cells["A1"].Value = "Aspose PDF Security Demo";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Использование #ctor для создания экземпляра PdfSecurityOptions.
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
            
            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.PrintPermission = true;
            pdfSecurityOptions.FullQualityPrintPermission = true;
            
            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            
            wb.Save("SecuredOutput.pdf", pdfSaveOptions);
            
            Console.WriteLine("PDF with security options created successfully.");
        }
    }
}
```

### См. также

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


