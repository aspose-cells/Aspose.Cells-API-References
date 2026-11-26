---
title: "GroupShape.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad GroupShape. Obtiene la forma hija por índice"
type: docs
url: /es/net/aspose.cells.drawing/groupshape/item/
---
## GroupShape indexer

Obtiene la forma hija por índice.

```csharp
public Shape this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | el índice de la forma hija. |

### Valor de retorno

devuelve la forma hija.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GroupShapePropertyItemDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear dos formas rectangulares
            Shape shape1 = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 0, 0);
            Shape shape2 = worksheet.Shapes.AddRectangle(50, 50, 100, 100, 0, 0);

            // Agrupar las formas
            Shape[] shapesToGroup = new Shape[] { shape1, shape2 };
            GroupShape groupShape = worksheet.Shapes.Group(shapesToGroup);

            // Acceder y mostrar las propiedades de la primera forma
            Shape firstShape = groupShape[0];
            Console.WriteLine($"First shape initial name: {firstShape.Name}");
            Console.WriteLine($"First shape initial text: {firstShape.Text}");

            // Modificar las propiedades de la primera forma mediante el acceso a Item
            firstShape.Name = "ModifiedRectangle1";
            firstShape.Text = "First Grouped Shape";

            // Acceder y modificar la segunda forma directamente mediante el indexador
            groupShape[1].Text = "Second Grouped Shape";

            // Verificar cambios
            Console.WriteLine($"\nFirst shape updated name: {groupShape[0].Name}");
            Console.WriteLine($"First shape updated text: {groupShape[0].Text}");
            Console.WriteLine($"Second shape updated text: {groupShape[1].Text}");

            // Guardar el libro de trabajo modificado
            workbook.Save("GroupShapePropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* class [GroupShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


