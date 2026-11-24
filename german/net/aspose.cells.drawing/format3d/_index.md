---
title: "Klasse Format3D"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.Format3D Klasse. Diese Klasse gibt die 3D‑Formeigenschaften für ein Diagrammelement oder eine Form an."
type: docs
url: /de/net/aspose.cells.drawing/format3d/
---
## Format3D class

Diese Klasse legt die 3D-Formeigenschaften für ein Diagrammelement oder eine Form fest.

```csharp
public class Format3D
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [LightingAngle](../../aspose.cells.drawing/format3d/lightingangle/) { get; set; } | Liest und setzt den Beleuchtungswinkel. Bereich von 0 bis 359,9 Grad. |
| [SurfaceLightingType](../../aspose.cells.drawing/format3d/surfacelightingtype/) { get; set; } | Liest und setzt den Beleuchtungstyp, der auf die Szene der Form angewendet wird. Standardwert ist LightRigType.ThreePoint. |
| [SurfaceMaterialType](../../aspose.cells.drawing/format3d/surfacematerialtype/) { get; set; } | Liest und setzt den Materialtyp, der mit den Beleuchtungseigenschaften kombiniert wird, um das endgültige Aussehen einer Form zu erzeugen. Standardwert ist PresetMaterialType.WarmMatte. |
| [TopBevel](../../aspose.cells.drawing/format3d/topbevel/) { get; } | Liest das [`Bevel`](../bevel/)‑Objekt, das die Eigenschaften enthält, die mit der Definition einer Abschrägung an der oberen oder vorderen Fläche einer Form verbunden sind. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [HasTopBevelData](../../aspose.cells.drawing/format3d/hastopbeveldata/)() | Gibt an, ob die Form obere Abschrägungsdaten enthält. |

### Beispiele

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class Format3DDemo
    {
        public static void RunDemo()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Serie zum Diagramm hinzufügen
            chart.NSeries.Add("A1:A4", true);

            // Zugriff auf die erste Serie
            Series series = chart.NSeries[0];

            // Greifen Sie auf das 3D-Format der Serie zu
            Format3D format3D = series.ShapeProperties.Format3D;

            // Setzen Sie die 3D‑Format-Eigenschaften
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Prüfen Sie, ob die Form obere Abschrägungsdaten hat
            if (format3D.HasTopBevelData())
            {
                Bevel topBevel = format3D.TopBevel;
                Console.WriteLine("Top Bevel Width: " + topBevel.Width);
                Console.WriteLine("Top Bevel Height: " + topBevel.Height);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("Format3DDemo.xlsx");
            workbook.Save("Format3DDemo.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


