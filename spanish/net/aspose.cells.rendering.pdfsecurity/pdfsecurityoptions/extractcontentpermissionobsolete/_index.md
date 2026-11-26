---
title: "PdfSecurityOptions.ExtractContentPermissionObsolete"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Permiso para copiar o extraer contenido obsoleto según la referencia PDF"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermissionobsolete/
---
## PdfSecurityOptions.ExtractContentPermissionObsolete property

Permiso para copiar o extraer contenido obsoleto según la referencia PDF.

```csharp
[Obsolete("Use ExtractContentPermission property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ExtractContentPermissionObsolete { get; set; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use la propiedad ExtractContentPermission. Esta propiedad será eliminada 12 meses después a partir de septiembre de 2023. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyExtractContentPermissionObsoleteDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.ExtractContentPermissionObsolete = false;
            pdfSecurityOptions.ExtractContentPermission = true;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("SecurePDF.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ExtractContentPermissionObsolete set to false");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


