---
title: "ThreeDFormat.ContourWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ThreeDFormat. Obtiene y establece el ancho del contorno en la forma en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing/threedformat/contourwidth/
---
## ThreeDFormat.ContourWidth property

Obtiene y establece el ancho del contorno en la forma, en unidades de puntos.

```csharp
public double ContourWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ThreeDFormatPropertyContourWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Agrega una forma a la hoja de cálculo con todos los parámetros requeridos
            Shape sh = ws.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);

            // Aplicar formato 3D
            ThreeDFormat n3df = sh.ThreeDFormat;
            n3df.ContourWidth = 17;
            n3df.ExtrusionHeight = 32;
            n3df.TopBevelType = (BevelType)BevelPresetType.HardEdge;

            // Guarda el libro de trabajo
            wb.Save("output.xlsx");

            // Verificar los valores guardados
            Workbook wb2 = new Workbook("output.xlsx");
            Shape sh2 = wb2.Worksheets[0].Shapes[0];
            ThreeDFormat n3df2 = sh2.ThreeDFormat;

            Console.WriteLine("ContourWidth: " + n3df2.ContourWidth);
            Console.WriteLine("ExtrusionHeight: " + n3df2.ExtrusionHeight);
            Console.WriteLine("TopBevelType: " + n3df2.TopBevelType);
        }
    }
}
```

### Ver también

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


