---
title: "ShapeCollection.AddSignatureLine"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Добавляет строку подписи в рабочий лист"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/addsignatureline/
---
## ShapeCollection.AddSignatureLine method

Добавляет строку подписи на лист.

```csharp
public Picture AddSignatureLine(int topRow, int leftColumn, SignatureLine signatureLine)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| topRow | Int32 | Индекс строки в верхнем левом углу. |
| leftColumn | Int32 | Индекс столбца в верхнем левом углу. |
| signatureLine | SignatureLine | Представляет объект строки подписи. |

### Примеры

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

### См. также

* class [Picture](../../picture/)
* class [SignatureLine](../../signatureline/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


