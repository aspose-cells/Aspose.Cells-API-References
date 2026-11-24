---
title: "PdfSecurityOptions.PdfSecurityOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfSecurityOptions-Konstruktor. Der Konstruktor von PdfSecurityOptions."
type: docs
url: /de/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/pdfsecurityoptions/
---
## PdfSecurityOptions constructor

Der Konstruktor von PdfSecurityOptions

```csharp
public PdfSecurityOptions()
```

### Beispiele

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
            
            // Verwenden von #ctor zum Erstellen einer PdfSecurityOptions-Instanz.
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

### Siehe auch

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


