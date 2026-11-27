---
title: "Shape.LineFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Returnerar ett MsoLineFormat-objekt som innehåller linjeformateringsegenskaper för den angivna formen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

Returnerar ett MsoLineFormat-objekt som innehåller linjeformateringsegenskaper för den angivna formen.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället Shape.Line-egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan juli 2016. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till en rektangelform i det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            RectangleShape rectangle = worksheet.Shapes.AddRectangle(3, 0, 2, 0, 70, 130);
            
            // Ställ in shape-egenskaper
            rectangle.Placement = PlacementType.FreeFloating;
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            
            // Demonstrera användning av LineFormat
            rectangle.LineFormat.Weight = 3; // Set line weight
            rectangle.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            rectangle.Line.SolidFill.Color = System.Drawing.Color.DarkBlue; // Correct way to set line color
            
            // Spara arbetsboken
            workbook.Save("ShapeLineFormatDemo.xlsx");
        }
    }
}
```

### Se även

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


