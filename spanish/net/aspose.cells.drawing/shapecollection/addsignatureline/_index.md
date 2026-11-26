---
title: "ShapeCollection.AddSignatureLine"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ShapeCollection método. Agrega una línea de firma a la hoja de cálculo"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addsignatureline/
---
## ShapeCollection.AddSignatureLine method

Agrega una Línea de Firma a la hoja de cálculo.

```csharp
public Picture AddSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| topRow | Int32 | Índice de fila superior izquierda. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| signatureLine | SignatureLine | Representa un objeto de línea de firma. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddSignatureLineWithInt32Int32SignatureLineDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            SignatureLine signatureLine = new SignatureLine();
            signatureLine.AllowComments = true;
            signatureLine.Email = "example@example.com";
            signatureLine.Instructions = "Sign to confirm the excel content.";
            signatureLine.IsLine = true;
            signatureLine.ShowSignedDate = true;
            signatureLine.Signer = "User";
            signatureLine.Title = "tester";

            Picture addedSignature = shapes.AddSignatureLine(100, 100, signatureLine);
            
            workbook.Save("SignatureLineDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Picture](../../picture/)
* class [SignatureLine](../../signatureline/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


