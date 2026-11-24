---
title: "Aufzählung DisplayUnitType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.DisplayUnitType enum. Stellt den Typ der Anzeigeeinheit der Diagrammachse dar"
type: docs
url: /de/net/aspose.cells.charts/displayunittype/
---
## DisplayUnitType enumeration

Stellt den Typ der Anzeigeeinheit der Diagrammachse dar.

```csharp
public enum DisplayUnitType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| None | `0` | Anzeigeeinheit ist Keine. |
| Hundreds | `1` | Gibt an, dass die Werte im Diagramm durch 100 geteilt werden. |
| Thousands | `2` | Gibt an, dass die Werte im Diagramm durch 1.000 geteilt werden. |
| TenThousands | `3` | Gibt an, dass die Werte im Diagramm durch 10.000 geteilt werden. |
| HundredThousands | `4` | Gibt an, dass die Werte im Diagramm durch 100.000 geteilt werden. |
| Millions | `5` | Gibt an, dass die Werte im Diagramm durch 1.000.000 geteilt werden. |
| TenMillions | `6` | Gibt an, dass die Werte im Diagramm durch 10.000.000 geteilt werden. |
| HundredMillions | `7` | Gibt an, dass die Werte im Diagramm durch 100.000.000 geteilt werden. |
| Billions | `8` | Gibt an, dass die Werte im Diagramm durch 1.000.000.000 geteilt werden. |
| Trillions | `9` | Gibt an, dass die Werte im Diagramm durch 1.000.000.000.000 dividiert werden sollen. |
| Percentage | `10` | Die Werte im Diagramm sollen durch 0,01 dividiert werden. |
| Cust | `11` | gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an. |
| Custom | `12` | gibt einen benutzerdefinierten Wert für die Anzeigeeinheit an. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitTypeDemo
    {
        public static void DisplayUnitTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Ein neues Arbeitsblatt zur Arbeitsmappe hinzufügen
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Füge einige Beispieldaten zum Arbeitsblatt hinzu
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Füge NSeries (Diagrammdatenquelle) zum Diagramm hinzu, das vom Feld "A1" bis "B3" reicht.
            chart.NSeries.Add("A1:B3", true);
            
            // Setzen Sie die Anzeigeeinheit der Werteachse auf Millionen
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            
            // Optional das Anzeigeeinheiten‑Label anzeigen
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // Speichere die Arbeitsmappe
            workbook.Save("DisplayUnitTypeExample.xlsx");
            workbook.Save("DisplayUnitTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


