---
title: "PdfSecurityOptions.AssembleDocumentPermission"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Indica si se permite ensamblar el documento (insertar, rotar o eliminar páginas) y crear marcadores o imágenes en miniatura incluso si ModifyDocumentPermission está habilitado"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/assembledocumentpermission/
---
## PdfSecurityOptions.AssembleDocumentPermission property

Indica si se permite ensamblar el documento (insertar, rotar o eliminar páginas y crear marcadores o imágenes en miniatura), incluso si [`ModifyDocumentPermission`](../modifydocumentpermission/) está habilitado.

```csharp
public bool AssembleDocumentPermission { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAssembleDocumentPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();

            pdfSecurityOptions.OwnerPassword = "owner123";
            pdfSecurityOptions.UserPassword = "user123";
            pdfSecurityOptions.AssembleDocumentPermission = false;
            pdfSecurityOptions.PrintPermission = true;

            pdfSaveOptions.SecurityOptions = pdfSecurityOptions;
            workbook.Save("secured_document.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with assemble document permission disabled.");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


