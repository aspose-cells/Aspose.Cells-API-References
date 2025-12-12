---
title: Aspose::Cells::Drawing::ShapeCollection::AddSignatureLine method
linktitle: AddSignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::ShapeCollection::AddSignatureLine method. Adds a Signature Line to the worksheet in C++.'
type: docs
weight: 5400
url: /cpp/aspose.cells.drawing/shapecollection/addsignatureline/
---
## ShapeCollection::AddSignatureLine method


Adds a Signature [Line](../../line/) to the worksheet.

```cpp
Aspose::Cells::Drawing::Picture Aspose::Cells::Drawing::ShapeCollection::AddSignatureLine(int32_t topRow, int32_t leftColumn, const SignatureLine &signatureLine)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |
| signatureLine | const SignatureLine\& | Represents a signature line object. |

## ReturnValue




## Examples


```cpp
SignatureLine wSignatureLine;
wSignatureLine.SetAllowComments(true);
wSignatureLine.SetEmail(u"example@example.com");
wSignatureLine.SetInstructions(u"Sign to confirm the excel content.");
wSignatureLine.SetIsLine(true);
wSignatureLine.SetShowSignedDate(true);
wSignatureLine.SetSigner(u"User");
wSignatureLine.SetTitle(u"tester");
//wSignatureLine.SignatureLineType = SignatureType.Stamp;
Picture signatureLine1 = shapes.AddSignatureLine(0, 0, wSignatureLine);
```

## See Also

* Class [Picture](../../picture/)
* Class [Vector](../../../aspose.cells/vector/)
* Class [SignatureLine](../../signatureline/)
* Class [ShapeCollection](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
