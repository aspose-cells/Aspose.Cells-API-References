---
title: "Format3D.HasTopBevelData"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Format3D-Methode. Gibt an, ob die Form obere Abschrägungsdaten hat"
type: docs
url: /de/net/aspose.cells.drawing/format3d/hastopbeveldata/
---
## Format3D.HasTopBevelData method

Gibt an, ob die Form obere Abschrägungsdaten enthält.

```csharp
public bool HasTopBevelData()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class Format3DMethodHasTopBevelDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);

            // Erstellen Sie ein 3D-Diagramm
            int chartIndex = sheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);

            // 3D-Format abrufen
            Format3D format3D = chart.NSeries[0].ShapeProperties.Format3D;

            // Obere Abschrägung festlegen
            format3D.TopBevel.Type = BevelPresetType.Circle;
            format3D.TopBevel.Width = 6;
            format3D.TopBevel.Height = 6;

            // Abschrägungsdaten prüfen und anzeigen
            if (format3D.HasTopBevelData())
            {
                Console.WriteLine("Top Bevel Type: " + format3D.TopBevel.Type);
                Console.WriteLine("Top Bevel Width: " + format3D.TopBevel.Width);
                Console.WriteLine("Top Bevel Height: " + format3D.TopBevel.Height);
            }

            workbook.Save("Format3DTopBevelDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


