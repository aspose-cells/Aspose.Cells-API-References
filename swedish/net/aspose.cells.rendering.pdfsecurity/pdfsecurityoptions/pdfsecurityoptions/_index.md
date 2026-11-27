---
title: "PdfSecurityOptions.PdfSecurityOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfSecurityOptions konstruktor. Konstruktor för PdfSecurityOptions"
type: docs
url: /sv/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/pdfsecurityoptions/
---
## PdfSecurityOptions constructor

Konstruktorn för PdfSecurityOptions

```csharp
public PdfSecurityOptions()
```

### Exempel

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
            
            // Använd #ctor för att skapa en PdfSecurityOptions-instans
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

### Se även

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


