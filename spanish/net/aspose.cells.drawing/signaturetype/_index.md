---
title: "Enumeración SignatureType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.SignatureType. Especifica el tipo de firma"
type: docs
url: /es/net/aspose.cells.drawing/signaturetype/
---
## SignatureType enumeration

Especifica el tipo de firma.

```csharp
public enum SignatureType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Default | `0` | El valor predeterminado, el valor correspondiente de ProviderId está fijado a {0000000000-0000-0000-0000-0000000000}. |
| Stamp | `1` | El valor correspondiente de ProviderId suele ser {000CD6A4-0000-0000-C000-000000000046}. |
| Custom | `3` | El valor correspondiente de ProviderId normalmente debe ser establecido por el usuario. Debe obtenerse de la documentación suministrada con el proveedor. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassSignatureTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar líneas de firma con diferentes tipos
            Picture stampPicture = worksheet.Shapes.AddSignatureLine(3, 1, new SignatureLine());
            stampPicture.SignatureLine.SignatureLineType = SignatureType.Stamp;

            Picture customPicture = worksheet.Shapes.AddSignatureLine(8, 1, new SignatureLine());
            customPicture.SignatureLine.SignatureLineType = SignatureType.Custom;
            customPicture.SignatureLine.ProviderId = new Guid("12345678-ABCD-4321-5678-9876543210AB");

            // Guardar el libro de trabajo con configuraciones de firma
            workbook.Save("SignatureTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


