---
title: "PdfSecurityOptions.PdfSecurityOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PdfSecurityOptions costruttore. Il costruttore di PdfSecurityOptions"
type: docs
url: /it/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/pdfsecurityoptions/
---
## PdfSecurityOptions constructor

Il costruttore di PdfSecurityOptions

```csharp
public PdfSecurityOptions()
```

### Esempi

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
            
            // Utilizzo di #ctor per creare un'istanza di PdfSecurityOptions
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

### Vedi anche

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


