---
title: "Enum ErrorBarType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.ErrorBarType enum. Stellt den Fehlerbalken-Mengen-Typ dar"
type: docs
url: /de/net/aspose.cells.charts/errorbartype/
---
## ErrorBarType enumeration

Stellt den Betragstyp der Fehlermarge dar.

```csharp
public enum ErrorBarType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Custom | `0` | InnerCustom Werttyp. |
| FixedValue | `1` | Fester Werttyp. |
| Percent | `2` | Prozenttyp |
| StDev | `3` | Standardabweichungstyp. |
| StError | `4` | Standardfehler‑Typ. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarTypeDemo
    {
        public static void ErrorBarTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Fügen Sie einige Beispieldaten hinzu
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);

            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Fehlerbalken‑Eigenschaften für jede Serie im Diagramm festlegen
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ErrorBarTypeExample.xlsx");
            workbook.Save("ErrorBarTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


