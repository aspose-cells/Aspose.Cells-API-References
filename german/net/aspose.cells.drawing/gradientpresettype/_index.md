---
title: "Enum GradientPresetType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.GradientPresetType-Enum. Stellt den Typ der voreingestellten Farbverläufe dar"
type: docs
url: /de/net/aspose.cells.drawing/gradientpresettype/
---
## GradientPresetType enumeration

Stellt den voreingestellten Farbtyp des Gradienten dar.

```csharp
public enum GradientPresetType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Brass | `0` | Messing-Voreinstellungsfarbe |
| CalmWater | `1` | Ruhiges Wasser-Voreinstellungsfarbe |
| Chrome | `2` | Chrom-Voreinstellungsfarbe |
| ChromeII | `3` | Chrome II Vorgabefarbe |
| Daybreak | `4` | Morgendämmerung Vorgabefarbe |
| Desert | `5` | Wüsten Vorgabefarbe |
| EarlySunset | `6` | Früher Sonnenuntergang Vorgabefarbe |
| Fire | `7` | Feuer Vorgabefarbe |
| Fog | `8` | Nebel Vorgabefarbe |
| Gold | `9` | Gold Vorgabefarbe |
| GoldII | `10` | Gold II Vorgabefarbe |
| Horizon | `11` | Horizont Vorgabefarbe |
| LateSunset | `12` | Später Sonnenuntergang Vorgabefarbe |
| Mahogany | `13` | Mahagoni Vorgabefarbe |
| Moss | `14` | Moos Vorgabefarbe |
| Nightfall | `15` | Nachtfall Vorgabefarbe |
| Ocean | `16` | Ozean Vorgabefarbe |
| Parchment | `17` | Pergament Vorgabefarbe |
| Peacock | `18` | Pfau Vorgabefarbe |
| Rainbow | `19` | Regenbogen Vorgabefarbe |
| RainbowII | `20` | Regenbogen II Vorgabefarbe |
| Sapphire | `21` | Saphir Vorgabefarbe |
| Silver | `22` | Silber Vorgabefarbe |
| Wheat | `23` | Weizen Vorgabefarbe |
| Unknown | `24` | Unbekannte Vorgabefarbe. Nur für die Vorgabefarbe (die nicht mit einer bekannten Vorgabefarbe übereinstimmt) in der Vorlagenarbeitsmappe. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientPresetTypeDemo
    {
        public static void GradientPresetTypeExample()
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

            // Zugriff auf die Kategorienachse des Diagramms
            Axis categoryAxis = chart.CategoryAxis;

            // Zugriff auf das Füllformat des Kategorienachsenbereichs
            FillFormat fillFormat = categoryAxis.Area.FillFormat;

            // Legen Sie eine Verlaufsvorgabefarbe für das Füllformat fest
            fillFormat.SetPresetColorGradient(GradientPresetType.Fire, GradientStyleType.Horizontal, 1);

            // Ausgabe des voreingestellten Farbverlaufs-Farbtyps
            Console.WriteLine("Gradient Preset Color: " + fillFormat.PresetColor);

            // Speichere die Arbeitsmappe
            workbook.Save("GradientPresetTypeExample.xlsx");
            workbook.Save("GradientPresetTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


