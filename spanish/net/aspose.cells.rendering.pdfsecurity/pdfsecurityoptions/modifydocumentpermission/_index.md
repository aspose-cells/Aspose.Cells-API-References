---
title: "PdfSecurityOptions.ModifyDocumentPermission"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Indica si se permite modificar el contenido del documento mediante operaciones distintas a las controladas por AnnotationsPermission, FillFormsPermission y AssembleDocumentPermission"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/modifydocumentpermission/
---
## PdfSecurityOptions.ModifyDocumentPermission property

Indica si se permite modificar el contenido del documento mediante operaciones distintas a las controladas por [`AnnotationsPermission`](../annotationspermission/), [`FillFormsPermission`](../fillformspermission/) y [`AssembleDocumentPermission`](../assembledocumentpermission/).

```csharp
public bool ModifyDocumentPermission { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyModifyDocumentPermissionDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Test PDF Security";

            // Configura las opciones de guardado de PDF con la configuración de seguridad
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Establece contraseñas y permisos
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.ModifyDocumentPermission = false; // Core property demonstration
            securityOptions.PrintPermission = true;

            // Aplica las opciones de seguridad y guarda
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredDocument.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ModifyDocumentPermission set to false");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


