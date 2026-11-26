---
title: "PdfSecurityOptions.PdfSecurityOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor PdfSecurityOptions. El constructor de PdfSecurityOptions"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/pdfsecurityoptions/
---
## PdfSecurityOptions constructor

El constructor de PdfSecurityOptions

```csharp
public PdfSecurityOptions()
```

### Ejemplos

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
            
            // Usando #ctor para crear una instancia de PdfSecurityOptions
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

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


