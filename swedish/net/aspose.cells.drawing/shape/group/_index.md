---
title: "Shape.Group"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar gruppfiguren som innehåller denna figur"
type: docs
url: /sv/net/aspose.cells.drawing/shape/group/
---
## Shape.Group property

Hämtar gruppformen som innehåller denna form.

```csharp
public GroupShape Group { get; }
```

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyGroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Skapa två exempelfigurer
            Shape shape1 = sheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 0);
            Shape shape2 = sheet.Shapes.AddOval(0, 100, 100, 100, 100, 0);

            // Gruppera figurerna med Shape-arrayparameter
            GroupShape group = sheet.Shapes.Group(new Shape[] { shape1, shape2 });

            // Åtkomst till gruppen via barnfigurens Group-egenskap
            GroupShape retrievedGroup = shape1.Group;
            
            // Demonstrera användning av Group-egenskapen
            retrievedGroup.Name = "MyShapeGroup";
            retrievedGroup.Placement = PlacementType.FreeFloating;

            workbook.Save("GroupShapeDemo.xlsx");
        }
    }
}
```

### Se även

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


