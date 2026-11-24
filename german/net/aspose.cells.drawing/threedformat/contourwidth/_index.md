---
title: "ThreeDFormat.ContourWidth"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreeDFormat-Eigenschaft. Liest und setzt die Konturbreite der Form in Einheit Punkte"
type: docs
url: /de/net/aspose.cells.drawing/threedformat/contourwidth/
---
## ThreeDFormat.ContourWidth property

Liest und setzt die Konturbreite der Form, in Punkten.

```csharp
public double ContourWidth { get; set; }
```

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];

            // Fügt dem Arbeitsblatt eine Form mit allen erforderlichen Parametern hinzu
            Shape sh = ws.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);

            // 3D-Formatierung anwenden
            ThreeDFormat n3df = sh.ThreeDFormat;
            n3df.ContourWidth = 17;
            n3df.ExtrusionHeight = 32;
            n3df.TopBevelType = (BevelType)BevelPresetType.HardEdge;

            // Speichere die Arbeitsmappe
            wb.Save("output.xlsx");

            // Überprüfe die gespeicherten Werte
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

### Siehe auch

* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


