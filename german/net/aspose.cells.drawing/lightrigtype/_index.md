---
title: "Aufzählung LightRigType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.LightRigType enum. Stellt ein voreingestelltes Licht rechts dar, das auf eine Form angewendet werden kann."
type: docs
url: /de/net/aspose.cells.drawing/lightrigtype/
---
## LightRigType enumeration

Stellt ein voreingestelltes Licht rechts dar, das auf eine Form angewendet werden kann

```csharp
public enum LightRigType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Balanced | `0` | Ausgewogen |
| BrightRoom | `1` | Heller Raum |
| Chilly | `2` | Kühl |
| Contrasting | `3` | Kontrastreich |
| Flat | `4` | Flach |
| Flood | `5` | Flut |
| Freezing | `6` | Eisig |
| Glow | `7` | Leuchten |
| Harsh | `8` | Hart |
| LegacyFlat1 | `9` | LegacyFlat1 |
| LegacyFlat2 | `10` | LegacyFlat2 |
| LegacyFlat3 | `11` | LegacyFlat3 |
| LegacyFlat4 | `12` | LegacyFlat4 |
| LegacyHarsh1 | `13` | LegacyHarsh1 |
| LegacyHarsh2 | `14` | LegacyHarsh2 |
| LegacyHarsh3 | `15` | LegacyHarsh3 |
| LegacyHarsh4 | `16` | LegacyHarsh4 |
| LegacyNormal1 | `17` | LegacyNormal1 |
| LegacyNormal2 | `18` | LegacyNormal2 |
| LegacyNormal3 | `19` | LegacyNormal3 |
| LegacyNormal4 | `20` | LegacyNormal4 |
| Morning | `21` | Morgen |
| Soft | `22` | Weich |
| Sunrise | `23` | Sonnenaufgang |
| Sunset | `24` | Sonnenuntergang |
| ThreePoint | `25` | Drei-Punkt |
| TwoPoint | `26` | Zwei-Punkt |
| None | `27` | Keine Lichtanlage. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LightRigTypeDemo
    {
        public static void LightRigTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Lege den Datenbereich des Diagramms fest
            chart.SetChartDataRange("A1:B4", true);

            // Greifen Sie auf die erste Serie im Diagramm zu
            Series series = chart.NSeries[0];

            // Greifen Sie auf die Formeigenschaften der Serie zu
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Überprüfen Sie, ob die Serie 3D-Formatdaten enthält
            if (shapeProperties.HasFormat3D())
            {
                // Greifen Sie auf die 3D-Formateigenschaften zu
                Format3D format3D = shapeProperties.Format3D;

                // Stellen Sie den Oberflächenbeleuchtungstyp auf Ausgewogen ein
                format3D.SurfaceLightingType = LightRigType.Balanced;

                // Stellen Sie den Beleuchtungswinkel ein
                format3D.LightingAngle = 45.0;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("LightRigTypeExample.xlsx");
            workbook.Save("LightRigTypeExample.pdf");
            // Ergebnisse ausgeben
            Console.WriteLine("LightRigType example applied and workbook saved as 'LightRigTypeExample.xlsx'.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


