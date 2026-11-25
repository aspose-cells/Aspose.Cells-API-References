---
title: "FillFormat.Scale"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FillFormat. Ottiene e imposta la scala del formato immagine"
type: docs
url: /it/net/aspose.cells.drawing/fillformat/scale/
---
## FillFormat.Scale property

Ottiene e imposta la scala del formato immagine.

```csharp
public double Scale { get; set; }
```

### Esempi

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

### Vedi anche

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


