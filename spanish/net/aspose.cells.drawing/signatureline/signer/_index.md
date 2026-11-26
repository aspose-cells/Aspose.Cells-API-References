---
title: "SignatureLine.Signer"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SignatureLine. Obtiene o establece el firmante"
type: docs
url: /es/net/aspose.cells.drawing/signatureline/signer/
---
## SignatureLine.Signer property

Obtiene o establece el firmante.

```csharp
public string Signer { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SignatureLinePropertySignerDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una línea de firma y establecer sus propiedades
            SignatureLine signatureLine = new SignatureLine();
            signatureLine.Signer = "John Doe";
            signatureLine.Title = "Software Developer";
            signatureLine.Email = "john.doe@example.com";

            // Agregar la línea de firma a la hoja de cálculo en la fila 1, columna 1
            worksheet.Shapes.AddSignatureLine(0, 0, signatureLine);

            // Guarda el libro de trabajo
            workbook.Save("SignatureLineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SignatureLine](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


