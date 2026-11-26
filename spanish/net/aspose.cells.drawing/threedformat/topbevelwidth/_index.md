---
title: "ThreeDFormat.TopBevelWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece el ancho del bisel superior o qué tan profundo se aplica en la forma. En unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/topbevelwidth/
---
## ThreeDFormat.TopBevelWidth property

Obtiene y establece el ancho del bisel superior, o cuán profundo se aplica en la forma. En unidades de puntos.

```csharp
public double TopBevelWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyTopBevelWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue una forma a la hoja de cálculo con los parámetros correctos
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 0, 0);

            // Obtener el formato 3D de la forma
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Establecer propiedades 3D incluyendo TopBevelWidth
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;
            threeDFormat.ContourWidth = 17;
            threeDFormat.ExtrusionHeight = 32;

            // Guarda el libro de trabajo
            workbook.Save("ThreeDFormatDemo.xlsx");

            // Verificar las propiedades guardadas
            Workbook loadedWorkbook = new Workbook("ThreeDFormatDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;

            Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
            Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
            Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
            Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


