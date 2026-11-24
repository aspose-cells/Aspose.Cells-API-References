---
title: "Shape.TextBody"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Einstellung des Textes des Shapes zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells.drawing/shape/textbody/
---
## Shape.TextBody property

Liest und setzt die Einstellung des Textes der Form.

```csharp
public FontSettingCollection TextBody { get; }
```

### Beispiele

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

### Siehe auch

* class [FontSettingCollection](../../../aspose.cells.drawing.texts/fontsettingcollection/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


