---
title: "Shape.Group"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Shape. Ottiene la forma di gruppo che contiene questa forma"
type: docs
url: /it/net/aspose.cells.drawing/shape/group/
---
## Shape.Group property

Ottiene la forma di gruppo che contiene questa forma.

```csharp
public GroupShape Group { get; }
```

### Esempi

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

            // Crea due forme di esempio
            Shape shape1 = sheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 0);
            Shape shape2 = sheet.Shapes.AddOval(0, 100, 100, 100, 100, 0);

            // Raggruppa le forme usando il parametro array Shape
            GroupShape group = sheet.Shapes.Group(new Shape[] { shape1, shape2 });

            // Accedi al gruppo tramite la proprietà Group della forma figlia
            GroupShape retrievedGroup = shape1.Group;
            
            // Dimostra l'uso della proprietà Group
            retrievedGroup.Name = "MyShapeGroup";
            retrievedGroup.Placement = PlacementType.FreeFloating;

            workbook.Save("GroupShapeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


