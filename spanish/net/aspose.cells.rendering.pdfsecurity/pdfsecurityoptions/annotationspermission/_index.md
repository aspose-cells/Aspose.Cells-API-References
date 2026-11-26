---
title: "PdfSecurityOptions.AnnotationsPermission"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Indica si se permite agregar o modificar anotaciones de texto y rellenar campos de formulario interactivos"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/annotationspermission/
---
## PdfSecurityOptions.AnnotationsPermission property

Indica si se permite agregar o modificar anotaciones de texto, rellenar campos de formulario interactivos.

```csharp
public bool AnnotationsPermission { get; set; }
```

### Observaciones

si [`ModifyDocumentPermission`](../modifydocumentpermission/) también está configurado, crear o modificar campos de formulario interactivos (incluidos los campos de firma).

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyAnnotationsPermissionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF with Annotations Permission";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.AnnotationsPermission = true;

            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("AnnotationsPermissionDemo.pdf", saveOptions);

            Console.WriteLine("PDF created with annotations permission enabled.");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


