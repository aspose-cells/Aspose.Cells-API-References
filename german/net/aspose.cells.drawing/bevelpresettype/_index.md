---
title: "Enum BevelPresetType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.BevelPresetType Enum. Stellt eine Vorgabe für einen Typ von Abschrägung dar, die auf eine Form in 3D angewendet werden kann"
type: docs
url: /de/net/aspose.cells.drawing/bevelpresettype/
---
## BevelPresetType enumeration

Stellt eine Voreinstellung für einen Abschrägungs‑Typ dar, die auf eine Form in 3D angewendet werden kann.

```csharp
public enum BevelPresetType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Keine Abschrägung |
| Angle | `1` | Winkel |
| ArtDeco | `2` | Art déco |
| Circle | `3` | Kreis |
| Convex | `4` | Konvex |
| CoolSlant | `5` | Coole Schräge |
| Cross | `6` | Kreuz |
| Divot | `7` | Kerbe |
| HardEdge | `8` | Harte Kante |
| RelaxedInset | `9` | Entspannte Einrückung |
| Riblet | `10` | Rippe |
| Slope | `11` | Steigung |
| SoftRound | `12` | Weiche Rundung |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class BevelPresetTypeDemo
    {
        public static void BevelPresetTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Arbeitsblatt hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich des Diagramms fest
            chart.SetChartDataRange("A1:B4", true);

            // Greifen Sie auf den Titel des Diagramms zu und setzen Sie dessen Text
            chart.Title.Text = "Sample Chart with Bevel";

            // Zugriff auf den Plotbereich des Diagramms
            PlotArea plotArea = chart.PlotArea;

            // Greifen Sie auf die Formeigenschaften des Plotbereichs zu
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            
            // Greifen Sie auf die 3D-Formateigenschaften zu
            Format3D format3D = shapeProperties.Format3D;

            // Greifen Sie auf die Eigenschaften der oberen Abschrägung zu
            Bevel topBevel = format3D.TopBevel;

            // Setzen Sie den Abschrägungstyp auf "Angle"
            topBevel.Type = BevelPresetType.Angle;

            // Setzen Sie die Breite und Höhe der Abschrägung
            topBevel.Width = 10;
            topBevel.Height = 10;

            // Speichere die Arbeitsmappe
            workbook.Save("BevelPresetTypeExample.xlsx");
            workbook.Save("BevelPresetTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


