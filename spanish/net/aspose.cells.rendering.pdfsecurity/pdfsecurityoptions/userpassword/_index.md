---
title: "PdfSecurityOptions.UserPassword"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfSecurityOptions. Obtiene o establece la contraseña de usuario requerida para abrir el documento PDF cifrado"
type: docs
url: /es/net/aspose.cells.rendering.pdfsecurity/pdfsecurityoptions/userpassword/
---
## PdfSecurityOptions.UserPassword property

Obtiene o establece la contraseña de usuario requerida para abrir el documento PDF encriptado.

```csharp
public string UserPassword { get; set; }
```

### Observaciones

Se requerirá la contraseña del propietario o la contraseña de usuario para abrir un documento PDF cifrado para su visualización.

La contraseña de usuario puede ser nula o una cadena vacía; en este caso no se requerirá contraseña al usuario al abrir el documento PDF.

Abrir el documento con la contraseña del propietario correcta permite acceso completo al documento.

Abrir el documento con la contraseña de usuario correcta (o abrir un documento que no tiene contraseña de usuario) permite acceso limitado según los permisos especificados.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering.PdfSecurity;

namespace AsposeCellsExamples
{
    public class PdfSecurityOptionsPropertyUserPasswordDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells["A1"].Value = "Protected PDF with User Password";

            PdfSaveOptions saveOptions = new PdfSaveOptions();
            PdfSecurityOptions securityOptions = new PdfSecurityOptions();
            
            securityOptions.UserPassword = "user123";
            securityOptions.OwnerPassword = "owner456";
            securityOptions.PrintPermission = true;
            
            saveOptions.SecurityOptions = securityOptions;
            workbook.Save("ProtectedWithUserPassword.pdf", saveOptions);
            
            Console.WriteLine("PDF created with user password protection.");
        }
    }
}
```

### Ver también

* class [PdfSecurityOptions](../)
* namespace [Aspose.Cells.Rendering.PdfSecurity](../../../aspose.cells.rendering.pdfsecurity/)
* assembly [Aspose.Cells](../../../)


