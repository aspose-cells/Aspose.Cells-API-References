---
title: "ShapeGuideCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ShapeGuideCollection. Obtiene una guía de forma por índice"
type: docs
url: /es/net/aspose.cells.drawing/shapeguidecollection/item/
---
## ShapeGuideCollection indexer

Obtiene una guía de forma por índice

```csharp
public ShapeGuide this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice |  |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añadir una forma que use guías de ajuste
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            // Acceder a la colección de guías de ajuste de la forma mediante Geometry
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

            // Añadir nuevas guías a la colección
            shapeGuides.Add("adj1", 25.5);
            shapeGuides.Add("adj2", 30);
            shapeGuides.Add("adj3", 25.5);
            shapeGuides.Add("adj4", 35);

            // Demostrar la lectura de valores de guía (propiedad Name no disponible en la definición proporcionada)
            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);

            // Guardar el libro de trabajo modificado
            workbook.Save("ShapeGuideCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeGuide](../../shapeguide/)
* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


