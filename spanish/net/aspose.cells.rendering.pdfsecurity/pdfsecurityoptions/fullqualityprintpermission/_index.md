---
title: "PdfSecurityOptions.FullQualityPrintPermission"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Indica si se permite imprimir el documento a una representación desde la cual se podría generar una copia digital fiel del contenido PDF."
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fullqualityprintpermission/
---
## PdfSecurityOptions.FullQualityPrintPermission property

Indica si se permite imprimir el documento a una representación a partir de la cual se pueda generar una copia digital fiel del contenido PDF.

```csharp
public bool FullQualityPrintPermission { get; set; }
```

### Observaciones

Cuando está habilitado (y [`PrintPermission`](../printpermission/) está configurado), la impresión se limita a una representación de bajo nivel del aspecto, posiblemente de calidad degradada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyFullQualityPrintPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test Full Quality Print Permission";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.FullQualityPrintPermission = true;
            securityOptions.PrintPermission = true;

            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("FullQualityPrintDemo.pdf", saveOptions);

            Console.WriteLine("PDF created with FullQualityPrintPermission enabled.");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


