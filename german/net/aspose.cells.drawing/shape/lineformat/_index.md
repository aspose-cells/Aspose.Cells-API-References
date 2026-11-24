---
title: "Shape.LineFormat"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt ein MsoLineFormat-Objekt zurück, das die Linienformatierungseigenschaften für die angegebene Form enthält"
type: docs
url: /de/net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

Gibt ein MsoLineFormat-Objekt zurück, das die Linienformatierungseigenschaften für die angegebene Form enthält.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Shape.Line-Eigenschaft. Diese Eigenschaft wird 12 Monate nach Juli 2016 entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyLineFormatDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügt dem ersten Arbeitsblatt ein Rechteck-Shape hinzu.
            Worksheet worksheet = workbook.Worksheets[0];
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
            
            // Formeigenschaften festlegen
            rectangle.Placement = PlacementType.FreeFloating;
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            
            // Demonstriere die Verwendung von LineFormat
            rectangle.LineFormat.Weight = 3; // Set line weight
            rectangle.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            rectangle.Line.SolidFill.Color = System.Drawing.Color.DarkBlue; // Correct way to set line color
            
            // Speichere die Arbeitsmappe
            workbook.Save("ShapeLineFormatDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


