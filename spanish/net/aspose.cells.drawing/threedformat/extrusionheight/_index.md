---
title: "ThreeDFormat.ExtrusionHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece la altura de extrusión aplicada a la forma en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/extrusionheight/
---
## ThreeDFormat.ExtrusionHeight property

Obtiene y establece la altura de extrusión aplicada a la forma, en unidades de puntos.

```csharp
public double ExtrusionHeight { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyExtrusionHeightDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de ejemplo con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);

            // Aplicar formato 3D
            ThreeDFormat threeDFormat = shape.ThreeDFormat;
            threeDFormat.ExtrusionHeight = 32;
            threeDFormat.ContourWidth = 17;
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Verificar los valores guardados
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;

            Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
            Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
            Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
            Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
            Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


