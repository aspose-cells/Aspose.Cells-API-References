---
title: "PdfSaveOptions.SecurityOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSaveOptions. Establezca estas opciones cuando se necesite seguridad en el resultado xls2pdf"
type: docs
url: /es/net/aspose.cells/pdfsaveoptions/securityoptions/
---
## PdfSaveOptions.SecurityOptions property

Establece estas opciones, cuando se necesita seguridad en el resultado xls2pdf.

```csharp
public PdfSecurityOptions SecurityOptions { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSaveOptionsPropertySecurityOptionsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de ejemplo
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF Demo";
            
            // Crea opciones de guardado PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Configurar opciones de seguridad
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;
            securityOptions.ExtractContentPermission = false;
            
            // Asignar opciones de seguridad a las opciones de guardado
            saveOptions.SecurityOptions = securityOptions;
            
            // Guardar el PDF con configuraciones de seguridad
            workbook.Save("SecuredDocument.pdf", saveOptions);
            
            Console.WriteLine("PDF with security options created successfully.");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../../../aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/)
* class [PdfSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


