---
title: "Bevel.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Bevel Eigenschaft. Gibt den voreingestellten Bevel-Typ zurück und legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/bevel/type/
---
## Bevel.Type property

Liest und setzt den voreingestellten Abschrägungstyp.

```csharp
public BevelPresetType Type { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdaten festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Erhalte die erste Serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];

            // Serienfarbe festlegen
            series.Area.ForegroundColor = Color.Blue;

            // 3D-Format und Bevel-Eigenschaften konfigurieren
            Format3D format3D = series.ShapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;

            // Demonstriere die Verwendung der Type‑Eigenschaft
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 5;
            topBevel.Height = 2;

            // Speichere die Arbeitsmappe
            workbook.Save("BevelPropertyTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [BevelPresetType](../../bevelpresettype/)
* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


