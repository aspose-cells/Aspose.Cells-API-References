---
title: "FillFormat.Scale"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство FillFormat. Получает и задает масштаб формата изображения"
type: docs
url: /ru/net/aspose.cells.drawing/fillformat/scale/
---
## FillFormat.Scale property

Получает и задает масштаб формата изображения.

```csharp
public double Scale { get; set; }
```

### Примеры

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyScaleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            RectangleShape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 150);
            shape1.Fill.FillType = FillType.Texture;
            shape1.Fill.Texture = TextureType.Denim;
            shape1.Fill.Scale = 50;

            RectangleShape shape2 = worksheet.Shapes.AddRectangle(0, 0, 2, 0, 100, 150);
            shape2.Fill.FillType = FillType.Texture;
            shape2.Fill.Texture = TextureType.Denim;
            shape2.Fill.Scale = 150;

            workbook.Save("FillFormatScaleDemo.xlsx");
        }
    }
}
```

### См. также

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


