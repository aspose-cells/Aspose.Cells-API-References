---
title: "ShapeCollection.AddSignatureLine"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ShapeCollection. يضيف سطر توقيع إلى ورقة العمل"
type: docs
url: /ar/net/aspose.cells.drawing/shapecollection/addsignatureline/
---
## ShapeCollection.AddSignatureLine method

يضيف خط توقيع إلى ورقة العمل.

```csharp
public Picture AddSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| topRow | Int32 | فهرس الصف العلوي الأيسر. |
| العمود الأيسر | Int32 | فهرس العمود العلوي الأيسر. |
| signatureLine | SignatureLine | يمثل كائن سطر توقيع. |

### أمثلة

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

### انظر أيضًا

* class [Picture](../../picture/)
* class [SignatureLine](../../signatureline/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


