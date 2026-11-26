---
title: "ShapeTextAlignment.TopMarginPt"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeTextAlignment. Возвращает верхний отступ в единицах точек"
type: docs
url: /ru/net/aspose.cells.drawing.texts/shapetextalignment/topmarginpt/
---
## ShapeTextAlignment.TopMarginPt property

Возвращает верхний отступ в единицах Points

```csharp
public double TopMarginPt { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentPropertyTopMarginPtDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);
            shape.Text = "Sample Text";
            
            shape.TextBody.TextAlignment.TopMarginPt = 2.0d;
            
            workbook.Save("ShapeTextAlignmentTopMarginPtDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


