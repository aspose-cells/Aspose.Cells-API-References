---
title: "Shape.Group"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Shape. Obtient la forme groupe qui contient cette forme"
type: docs
url: /fr/net/aspose.cells.drawing/shape/group/
---
## Shape.Group property

Obtient le groupe de formes qui contient cette forme.

```csharp
public GroupShape Group { get; }
```

### Exemples

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

            // Créer deux formes d'exemple
            Shape shape1 = sheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 0);
            Shape shape2 = sheet.Shapes.AddOval(0, 100, 100, 100, 100, 0);

            // Regrouper les formes en utilisant le paramètre de tableau Shape
            GroupShape group = sheet.Shapes.Group(new Shape[] { shape1, shape2 });

            // Accéder au groupe via la propriété Group de la forme enfant
            GroupShape retrievedGroup = shape1.Group;
            
            // Démontrer l'utilisation de la propriété Group
            retrievedGroup.Name = "MyShapeGroup";
            retrievedGroup.Placement = PlacementType.FreeFloating;

            workbook.Save("GroupShapeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


