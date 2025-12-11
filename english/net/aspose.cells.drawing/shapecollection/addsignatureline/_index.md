---
title: ShapeCollection.AddSignatureLine
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Adds a Signature Line to the worksheet
type: docs
url: /net/aspose.cells.drawing/shapecollection/addsignatureline/
---
## ShapeCollection.AddSignatureLine method

Adds a Signature Line to the worksheet.

```csharp
public Picture AddSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Int32 | Upper left row index. |
| leftColumn | Int32 | Upper left column index. |
| signatureLine | SignatureLine | Represents a signature line object. |

### Examples

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

### See Also

* class [Picture](../../picture/)
* class [SignatureLine](../../signatureline/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


