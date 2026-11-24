---
title: "Klasse Bevel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Bevel Klasse. Stellt eine Abschrägung einer Form dar"
type: docs
url: /de/net/aspose.cells.drawing/bevel/
---
## Bevel class

Stellt eine Abschrägung einer Form dar.

```csharp
public class Bevel
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Height](../../aspose.cells.drawing/bevel/height/) { get; set; } | Liest und setzt die Höhe der Abschrägung bzw. wie weit über der Form sie angewendet wird. In Punkten. |
| [Type](../../aspose.cells.drawing/bevel/type/) { get; set; } | Liest und setzt den voreingestellten Abschrägungstyp. |
| [Width](../../aspose.cells.drawing/bevel/width/) { get; set; } | Liest und setzt die Breite der Abschrägung bzw. wie weit in die Form sie angewendet wird. In Punkten. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class BevelDemo
    {
        public static void RunDemo()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            workbook.CalculateFormula();

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Datenreihen zum Diagramm hinzufügen
            chart.NSeries.Add("A1:B4", true);

            // Zugriff auf den Plotbereich des Diagramms
            ChartFrame plotArea = chart.PlotArea;

            // Greifen Sie auf die Formeigenschaften des Plotbereichs zu
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            // Greifen Sie auf die 3D-Formateigenschaften zu
            Format3D format3D = shapeProperties.Format3D;

            // Greifen Sie auf die Eigenschaften der oberen Abschrägung zu
            Bevel topBevel = format3D.TopBevel;

            // Setze Breite, Höhe und Typ der Abschrägung
            topBevel.Width = 10.0;
            topBevel.Height = 5.0;
            topBevel.Type = BevelPresetType.Circle;

            // Setze weitere 3D-Format-Eigenschaften
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Speichere die Arbeitsmappe
            workbook.Save("BevelDemo.xlsx");
            workbook.Save("BevelDemo.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


