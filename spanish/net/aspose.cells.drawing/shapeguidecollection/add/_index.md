---
title: "ShapeGuideCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeGuideCollection. Añade una guía de forma. Importante: esta característica está disponible actualmente solo para Excel07 y versiones posteriores"
type: docs
url: /es/net/aspose.cells.drawing/shapeguidecollection/add/
---
## ShapeGuideCollection.Add method

Agrega una guía de forma.(Importante: Esta característica está disponible actualmente solo para Excel07 y versiones posteriores)

```csharp
public int Add(string name, double val)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| name | String | el nombre de adjust. Es como "adj (Usado cuando hay un solo valor de ajuste)", "adj1", "adj2", "adj3" y así sucesivamente. |
| val | Double | el valor de adjust |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma que use guías de ajuste
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            try
            {
                // Obtener el ShapeGuideCollection de los ajustes de geometría de la forma
                ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

                // Llamar al método Add con parámetros (String, Double)
                shapeGuides.Add("adj1", 25.5);
                shapeGuides.Add("adj2", 25.5);
                shapeGuides.Add("adj3", 25.5);
                shapeGuides.Add("adj4", 25.5);

                Console.WriteLine($"Total guides after addition: {shapeGuides.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Guardar el libro de trabajo modificado
            workbook.Save("ShapeGuideAddWithStringDoubleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


