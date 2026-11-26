---
title: "PdfSecurityOptions.OwnerPassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Obtiene o establece la contraseña del propietario para el documento PDF cifrado"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/ownerpassword/
---
## PdfSecurityOptions.OwnerPassword property

Obtiene o establece la contraseña del propietario para el documento PDF encriptado.

```csharp
public string OwnerPassword { get; set; }
```

### Observaciones

La contraseña del propietario permite al usuario abrir un documento PDF cifrado sin ninguna restricción de acceso especificada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyOwnerPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with Owner Password";

            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();

            securityOptions.OwnerPassword = "owner123";
            securityOptions.UserPassword = "user123";
            securityOptions.PrintPermission = true;
            securityOptions.ModifyDocumentPermission = false;

            pdfSaveOptions.SecurityOptions = securityOptions;
            workbook.Save("SecuredPdfWithOwnerPassword.pdf", pdfSaveOptions);

            Console.WriteLine("PDF created with owner password protection.");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


