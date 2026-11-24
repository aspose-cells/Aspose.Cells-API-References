---
title: "ThreeDFormat.TopBevelWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Liest und setzt die Breite des oberen Abschrägungsbereichs bzw. wie weit sie auf die Form angewendet wird. In Einheit Punkte"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/topbevelwidth/
---
## ThreeDFormat.TopBevelWidth property

Liest und setzt die Breite der oberen Abschrägung bzw. wie tief sie in die Form eingreift. In Punkten.

```csharp
public double TopBevelWidth { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie ein Shape dem Arbeitsblatt mit korrekten Parametern hinzu.
            Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 0, 0);

            // Erhalte das 3D-Format der Form
            ThreeDFormat threeDFormat = shape.ThreeDFormat;

            // Setze 3D-Eigenschaften einschließlich TopBevelWidth
            threeDFormat.TopBevelType = BevelType.HardEdge;
            threeDFormat.TopBevelWidth = 30;
            threeDFormat.TopBevelHeight = 30;
            threeDFormat.ContourWidth = 17;
            threeDFormat.ExtrusionHeight = 32;

            // Speichere die Arbeitsmappe
            workbook.Save("ThreeDFormatDemo.xlsx");

            // Überprüfe die gespeicherten Eigenschaften
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

### Siehe auch

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


