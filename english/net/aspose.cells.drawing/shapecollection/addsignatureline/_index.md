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
public Picture AddSignatureLine(int upperLeftRow, int upperLeftColumn, SignatureLine signatureLine)
```

| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | Int32 | Upper left row index. |
| upperLeftColumn | Int32 | Upper left column index. |
| signatureLine | SignatureLine | Represents a signature line object. |

### Examples

```csharp

[C#]
SignatureLine wSignatureLine = new SignatureLine();
wSignatureLine.AllowComments = true;
wSignatureLine.Email = "dsltak@gmail.com";
wSignatureLine.Instructions = "Sign to confirm the excel content.";
wSignatureLine.IsLine = true;
wSignatureLine.ShowSignedDate = true;
wSignatureLine.Signer = "TAKYU";
wSignatureLine.Title = "tester";
//wSignatureLine.SignatureLineType = SignatureType.Stamp;
Picture signatureLine1 = gWS.Shapes.AddSignatureLine(0, 0, wSignatureLine);

```

### See Also

* class [Picture](../../picture/)
* class [SignatureLine](../../signatureline/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


