---
title: "Shape.TextBody"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger inställningen för formens text"
type: docs
url: /sv/net/aspose.cells.drawing/shape/textbody/
---
## Shape.TextBody property

Hämtar och anger inställningen för formens text.

```csharp
public FontSettingCollection TextBody { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapePropertyTextBodyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 200);
            FontSettingCollection fontSettingCollection = shape.TextBody;
            fontSettingCollection.Text = "This is a test.";

            workbook.Save("ShapeTextBodyDemo.xlsx");
        }
    }
}
```

### Se även

* class [FontSettingCollection](../../../aspose.cells.drawing.texts/fontsettingcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


