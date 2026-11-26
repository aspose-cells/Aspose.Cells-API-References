---
title: "PdfSecurityOptions.ExtractContentPermission"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Indica si se permite copiar o extraer de otro modo texto y gráficos del documento mediante operaciones distintas a las controladas por AccessibilityExtractContent"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/extractcontentpermission/
---
## PdfSecurityOptions.ExtractContentPermission property

Indica si se permite copiar o extraer de otro modo texto y gráficos del documento mediante operaciones distintas a las controladas por [`AccessibilityExtractContent`](../accessibilityextractcontent/).

```csharp
public bool ExtractContentPermission { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyExtractContentPermissionDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Sample PDF Content";

            // Configura las opciones de guardado de PDF con la configuración de seguridad
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            // Establece contraseñas y permisos
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            
            // Demuestra el uso de ExtractContentPermission
            securityOptions.ExtractContentPermission = false;
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;

            // Aplica las opciones de seguridad y guarda
            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredPDF.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with ExtractContentPermission set to false");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


