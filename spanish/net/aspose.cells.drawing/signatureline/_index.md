---
title: "Clase SignatureLine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.SignatureLine. Representa la línea de firma"
type: docs
url: /es/net/aspose.cells.drawing/signatureline/
---
## SignatureLine class

Representa la línea de firma.

```csharp
public class SignatureLine
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [SignatureLine](signatureline/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AllowComments](../../aspose.cells.drawing/signatureline/allowcomments/) { get; set; } | Indica si se pueden adjuntar comentarios. |
| [Email](../../aspose.cells.drawing/signatureline/email/) { get; set; } | Obtiene o establece el correo electrónico del cantante. |
| [Id](../../aspose.cells.drawing/signatureline/id/) { get; set; } | Obtiene o establece el identificador de esta línea de firma. |
| [Instructions](../../aspose.cells.drawing/signatureline/instructions/) { get; set; } | Obtiene o establece el texto mostrado al usuario al firmar. |
| [IsLine](../../aspose.cells.drawing/signatureline/isline/) { get; set; } | Indica si es una línea de firma. |
| [ProviderId](../../aspose.cells.drawing/signatureline/providerid/) { get; set; } | Obtiene o establece el id del proveedor de firma. |
| [ShowSignedDate](../../aspose.cells.drawing/signatureline/showsigneddate/) { get; set; } | Indica si se muestra la fecha de firma. |
| [SignatureLineType](../../aspose.cells.drawing/signatureline/signaturelinetype/) { get; set; } | Obtiene o establece el tipo de firma. Default - Cuando se establece el valor predeterminado, el valor correspondiente de ProviderId se fija a {0000000000-0000-0000-0000-0000000000}. Stamp - Cuando el valor es Stamp, el valor correspondiente de ProviderId suele ser {000CD6A4-0000-0000-C000-000000000046}. Custom - Cuando el valor es Custom, el valor correspondiente de ProviderId normalmente debe ser establecido por el usuario. debe obtenerse de la documentación suministrada con el proveedor. |
| [Signer](../../aspose.cells.drawing/signatureline/signer/) { get; set; } | Obtiene o establece el firmante. |
| [Title](../../aspose.cells.drawing/signatureline/title/) { get; set; } | Obtiene o establece el título del cantante. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLineDemo
    {
        public static void SignatureLineExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una imagen
            int imgIndex = worksheet.Pictures.Add(1, 1, "SignatureLineExample_original.png");
            Picture pic = worksheet.Pictures[imgIndex];

            // Crear objeto de línea de firma
            SignatureLine s = new SignatureLine();
            s.Signer = "Simon Zhao";
            s.Title = "Development Lead";
            s.Email = "Simon.Zhao@aspose.com";
            s.Id = Guid.NewGuid();
            s.ProviderId = Guid.NewGuid();
            s.IsLine = true;
            s.AllowComments = true;
            s.ShowSignedDate = true;
            s.Instructions = "Just do it.";

            // Asignar el objeto de línea de firma a la propiedad Picture.SignatureLine
            pic.SignatureLine = s;

            // Guardar el archivo Excel
            workbook.Save("SignatureLineExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


