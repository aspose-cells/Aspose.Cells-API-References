---
title: "SignatureLine.SignatureLineType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SignatureLine. Obtiene o establece el tipo de firma. Default  Cuando el valor predeterminado se establece, el valor correspondiente de ProviderId se fija a 00000000000000000000000000000000. Stamp  Cuando el valor es Stamp, el valor correspondiente de ProviderId suele ser 000CD6A400000000C000000000000046. Custom  Cuando el valor es Custom, el valor correspondiente de ProviderId normalmente debe ser establecido por el usuario. debe obtenerse de la documentación suministrada con el proveedor"
type: docs
url: /es/net/aspose.cells.drawing/signatureline/signaturelinetype/
---
## SignatureLine.SignatureLineType property

Obtiene o establece el tipo de firma. Default - Cuando se establece el valor predeterminado, el valor correspondiente de ProviderId se fija a {0000000000-0000-0000-0000-0000000000}. Stamp - Cuando el valor es Stamp, el valor correspondiente de ProviderId suele ser {000CD6A4-0000-0000-C000-000000000046}. Custom - Cuando el valor es Custom, el valor correspondiente de ProviderId normalmente debe ser establecido por el usuario. debe obtenerse de la documentación suministrada con el proveedor.

```csharp
public SignatureType SignatureLineType { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class SignatureLinePropertySignatureLineTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una línea de firma
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Developer";
            signatureLine.Email = "john@example.com";
            signatureLine.IsLine = true;
            signatureLine.AllowComments = true;
            signatureLine.ShowSignedDate = true;
            signatureLine.Instructions = "Please sign here";

            // Mostrar el SignatureLineType actual
            Console.WriteLine("Current SignatureLineType: " + signatureLine.SignatureLineType);

            // Establecer SignatureLineType a Stamp
            signatureLine.SignatureLineType = SignatureType.Stamp;
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("ProviderId after Stamp type: " + signatureLine.ProviderId);

            // Agregar la línea de firma a la hoja de cálculo añadiéndola a las formas
            Picture signaturePicture = worksheet.Shapes.AddSignatureLine(0, 0, signatureLine); // Changed to Picture type
            Console.WriteLine("Added signature line with index: " + signaturePicture.OriginalHeight);

            // Cambiar SignatureLineType a Custom con ProviderId personalizado
            signatureLine.SignatureLineType = SignatureType.Custom;
            signatureLine.ProviderId = Guid.NewGuid();
            Console.WriteLine("Changed SignatureLineType to: " + signatureLine.SignatureLineType);
            Console.WriteLine("Custom ProviderId: " + signatureLine.ProviderId);

            // Guarda el libro de trabajo
            workbook.Save("SignatureLineTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SignatureType](../../signaturetype/)
* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


