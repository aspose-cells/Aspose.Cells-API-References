---
title: "Shape.Group"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Obtiene la forma de grupo que contiene esta forma"
type: docs
url: /es/net/aspose.cells.drawing/shape/group/
---
## Shape.Group property

Obtiene la forma de grupo que contiene esta forma.

```csharp
public GroupShape Group { get; }
```

### Ejemplos

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

            // Crear dos formas de muestra
            Shape shape1 = sheet.Shapes.AddRectangle(0, 0, 0, 100, 100, 0);
            Shape shape2 = sheet.Shapes.AddOval(0, 100, 100, 100, 100, 0);

            // Agrupar las formas usando el parámetro de matriz Shape
            GroupShape group = sheet.Shapes.Group(new Shape[] { shape1, shape2 });

            // Acceder al grupo a través de la propiedad Group de la forma hija
            GroupShape retrievedGroup = shape1.Group;
            
            // Demostrar el uso de la propiedad Group
            retrievedGroup.Name = "MyShapeGroup";
            retrievedGroup.Placement = PlacementType.FreeFloating;

            workbook.Save("GroupShapeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GroupShape](../../groupshape/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


