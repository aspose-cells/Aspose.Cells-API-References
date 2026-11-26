---
title: "Shape.IsInGroup"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Shape. Indica si la forma está agrupada"
type: docs
url: /es/net/aspose.cells.drawing/shape/isingroup/
---
## Shape.IsInGroup property

Indica si la forma está agrupada.

```csharp
public bool IsInGroup { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyIsInGroupDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunas formas con todos los parámetros requeridos (upperLeftRow, upperLeftColumn, height, width, imageWidth, imageHeight)
            Shape shape1 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 50, 100);
            Shape shape2 = worksheet.Shapes.AddRectangle(6, 0, 2, 0, 50, 100);
            Shape shape3 = worksheet.Shapes.AddRectangle(3, 0, 5, 0, 50, 100);

            // Agrupar las formas con los parámetros correctos
            GroupShape group = worksheet.Shapes.Group(new Shape[] { shape1, shape2, shape3 });

            // Verificar si las formas están en un grupo
            Console.WriteLine("Shape1 IsInGroup: " + shape1.IsInGroup);
            Console.WriteLine("Shape2 IsInGroup: " + shape2.IsInGroup);
            Console.WriteLine("Shape3 IsInGroup: " + shape3.IsInGroup);
            Console.WriteLine("GroupShape IsInGroup: " + group.IsInGroup);

            // Agregar una forma sin agrupar
            Shape ungroupedShape = worksheet.Shapes.AddRectangle(10, 0, 2, 0, 50, 100);
            Console.WriteLine("Ungrouped shape IsInGroup: " + ungroupedShape.IsInGroup);

            // Guardar el resultado
            workbook.Save("ShapePropertyIsInGroupDemo.xlsx");

            // Desagrupar las formas y obtener las formas desagrupadas del grupo
            group.Ungroup();
            Console.WriteLine("After ungrouping, shape1 IsInGroup: " + shape1.IsInGroup);
            Console.WriteLine("After ungrouping, shape2 IsInGroup: " + shape2.IsInGroup);
            Console.WriteLine("After ungrouping, shape3 IsInGroup: " + shape3.IsInGroup);

            // Guardar el resultado
            workbook.Save("ShapePropertyIsInGroupDemo2.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


