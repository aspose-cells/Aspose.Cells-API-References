---
title: "ShapeCollection.AddSignatureLine"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection‑metod. Lägger till en signaturlinje i kalkylbladet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addsignatureline/
---
## ShapeCollection.AddSignatureLine method

Lägger till en signaturlinje i kalkylbladet.

```csharp
public Picture AddSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| topRow | Int32 | Övre vänstra radindex. |
| leftColumn | Int32 | Övre vänstra kolumnindex. |
| signatureLine | SignatureLine | Representerar ett signaturlinje‑objekt. |

### Exempel

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

### Se även

* class [Picture](../../picture/)
* class [SignatureLine](../../signatureline/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


