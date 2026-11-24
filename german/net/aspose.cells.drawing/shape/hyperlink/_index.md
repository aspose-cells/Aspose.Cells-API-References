---
title: "Shape.Hyperlink"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt den Hyperlink der Form zurück."
type: docs
url: /de/net/aspose.cells.drawing/shape/hyperlink/
---
## Shape.Hyperlink property

Ruft den Hyperlink der Form ab.

```csharp
public Hyperlink Hyperlink { get; }
```

### Beispiele

```csharp
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapePropertyHyperlinkDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            Aspose.Cells.Drawing.Shape shape = sheet.Shapes.AddRectangle(0, 0, 10, 10, 100, 150);
            Hyperlink hyperlink = shape.Hyperlink;
            hyperlink.Address = "https://www.aspose.com";
            hyperlink.ScreenTip = "Click to open Aspose website";

            workbook.Save("ShapeHyperlinkDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


