---
title: "PdfSecurityOptions.FillFormsPermission"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Indica si se permite rellenar campos de formulario interactivo existentes, incluidos los campos de firma, incluso si ModifyDocumentPermission está desactivado"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/fillformspermission/
---
## PdfSecurityOptions.FillFormsPermission property

Indica si se permite rellenar campos de formulario interactivo existentes (incluidos los campos de firma), incluso si [`ModifyDocumentPermission`](../modifydocumentpermission/) está desactivado.

```csharp
public bool FillFormsPermission { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyFillFormsPermissionDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "PDF Form Example";

            // Configura las opciones de guardado de PDF con la configuración de seguridad
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Establece contraseñas y permisos
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.FillFormsPermission = true; // Key permission being demonstrated
            securityOptions.PrintPermission = true;

            // Aplica las opciones de seguridad y guarda
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecureFormFillEnabled.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with form filling permission enabled.");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


