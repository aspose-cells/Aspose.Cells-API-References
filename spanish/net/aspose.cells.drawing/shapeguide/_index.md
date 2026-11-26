---
title: "Clase ShapeGuide"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ShapeGuide. Encapsula una guía de forma que especifica la presencia de una guía de forma que se usará para gobernar la geometría de la forma especificada."
type: docs
url: /es/net/aspose.cells.drawing/shapeguide/
---
## ShapeGuide class

Encapsula una guía de forma que especifica la presencia de una guía de forma que se utilizará para gobernar la geometría de la forma especificada.

```csharp
public class ShapeGuide : BaseShapeGuide
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Value](../../aspose.cells.drawing/shapeguide/value/) { get; set; } | Obtiene o establece el valor de esta guía |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeGuideDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 0, 100, 100, 100, 100);
                
                // Crear y agregar una guía de forma con los parámetros requeridos
                int guideIndex = shape.Geometry.ShapeAdjustValues.Add("Guide1", 0.2);
                ShapeGuide guide = shape.Geometry.ShapeAdjustValues[guideIndex];
                
                Console.WriteLine($"ShapeGuide created with Value: {guide.Value}");
                
                workbook.Save("DrawingClassShapeGuideDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [BaseShapeGuide](../baseshapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


