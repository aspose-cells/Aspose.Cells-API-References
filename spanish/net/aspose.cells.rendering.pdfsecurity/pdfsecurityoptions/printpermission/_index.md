---
title: "PdfSecurityOptions.PrintPermission"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Indica si se permite imprimir el documento"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/printpermission/
---
## PdfSecurityOptions.PrintPermission property

Indica si se permite imprimir el documento.

```csharp
public bool PrintPermission { get; set; }
```

### Observaciones

Posiblemente no al nivel de mayor calidad, dependiendo de si [`FullQualityPrintPermission`](../fullqualityprintpermission/) también está activado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyPrintPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test Print Permission";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;

            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("PrintPermissionDemo.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with print permission enabled.");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


