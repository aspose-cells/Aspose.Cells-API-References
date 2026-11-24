---
title: "Shape.Group"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Shape-Eigenschaft. Gibt die Gruppenshape zurück, die diese Shape enthält"
type: docs
url: /de/net/aspose.cells.drawing/shape/group/
---
## Shape.Group property

Liest das Gruppenshape, das dieses Shape enthält

```csharp
public GroupShape Group { get; }
```

### Beispiele

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

            // Erstelle zwei Beispiel-Shapes
            Shape shape1 = sheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 0);
            Shape shape2 = sheet.Shapes.AddOval(0, 100, 100, 100, 100, 0);

            // Gruppiere die Shapes mithilfe des Shape-Array-Parameters
            GroupShape group = sheet.Shapes.Group(new Shape[] { shape1, shape2 });

            // Greife über die Group-Eigenschaft der Kind-Shape auf die Gruppe zu
            GroupShape retrievedGroup = shape1.Group;
            
            // Demonstriere die Verwendung der Group-Eigenschaft
            retrievedGroup.Name = "MyShapeGroup";
            retrievedGroup.Placement = PlacementType.FreeFloating;

            workbook.Save("GroupShapeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


