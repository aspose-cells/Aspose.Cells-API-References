---
title: "Aufzählung DataLabelsSeparatorType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.DataLabelsSeparatorType enum. Stellt den Trennzeichen‑Typ von Datenbeschriftungen dar"
type: docs
url: /de/net/aspose.cells.charts/datalabelsseparatortype/
---
## DataLabelsSeparatorType enumeration

Stellt den Trennertyp von DataLabels dar.

```csharp
public enum DataLabelsSeparatorType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Auto | `0` | Stellt automatisches Trennzeichen dar |
| Space | `1` | Stellt das Leerzeichen (" ") dar |
| Comma | `2` | Stellt das Komma (",") dar |
| Semicolon | `3` | Stellt ein Semikolon (";") dar |
| Period | `4` | Stellt den Punkt (".") dar |
| NewLine | `5` | Stellt den Zeilenumbruch ("\n") dar |
| Custom | `6` | Stellt ein benutzerdefiniertes Trennzeichen dar |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class DataLabelsSeparatorTypeDemo
    {
        public static void DataLabelsSeparatorTypeExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten für das Diagramm hinzu
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Füge dem Arbeitsblatt ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Füge die Datenreihe dem Diagramm hinzu
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Greife auf die Datenbeschriftungen der ersten Reihe zu
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Setze den Trennzeichen‑Typ auf Komma
            dataLabels.SeparatorType = DataLabelsSeparatorType.Comma;

            // Aktiviere Datenbeschriftungen und setze einige Eigenschaften
            dataLabels.ShowCategoryName = true;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.InsideBase;

            // Setze Schriftarteigenschaften
            dataLabels.Font.Color = Color.Blue;
            dataLabels.Font.IsBold = true;

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsSeparatorTypeExample.xlsx");
            workbook.Save("DataLabelsSeparatorTypeExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


