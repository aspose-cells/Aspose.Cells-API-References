---
title: "GroupShape.Ungroup"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método GroupShape. Desagrupa los elementos de la forma"
type: docs
url: /es/net/aspose.cells.drawing/groupshape/ungroup/
---
## GroupShape.Ungroup method

Desagrupa los elementos de la forma.

```csharp
public void Ungroup()
```

### Observaciones

Si la forma de grupo está agrupada por otra forma de grupo, no se hará nada.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapeMethodUngroupDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar dos formas rectangulares
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 50);
            Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 3, 0, 100, 50);

            // Agrupar formas en un GroupShape
            GroupShape groupShape = worksheet.Shapes.Group(new Shape[] { shape1, shape2 });

            try
            {
                // Ejecutar el método Ungroup
                groupShape.Ungroup();
                Console.WriteLine("Shapes ungrouped successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during ungrouping: {ex.Message}");
            }

            workbook.Save("GroupShapeUngroupDemo.xlsx");
        }
    }
}
```

### Ver también

* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


