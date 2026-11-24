---
title: "TrendlineCollection.Add"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TrendlineCollection-Methode. Fügt dieser Sammlung ein Trendline-Objekt mit dem angegebenen Typ hinzu"
type: docs
url: /de/net/aspose.cells.charts/trendlinecollection/add/
---
## Add(TrendlineType) {#add}

Fügt dieser Sammlung ein [`Trendline`](../../trendline/) Objekt mit dem angegebenen Typ hinzu.

```csharp
public int Add(TrendlineType type)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | TrendlineType | Trendline-Typ. |

### Rückgabewert

[`Trendline`](../../trendline/) object index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["B3"].PutValue(4);
            worksheet.Cells["B4"].PutValue(8);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Seriendaten hinzufügen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Exponentialen Trendline zur ersten Serie hinzufügen
            chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);

            // Speichere die Arbeitsmappe
            workbook.Save("TrendlineCollectionMethodAddWithTrendlineTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(TrendlineType, string) {#add_1}

Fügt dieser Sammlung ein [`Trendline`](../../trendline/) Objekt mit angegebenem Typ und Namen hinzu.

```csharp
public int Add(TrendlineType type, string name)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | TrendlineType | Trendline-Typ. |
| Name | String | Trendline-Name. |

### Rückgabewert

[`Trendline`](../../trendline/) object index.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionMethodAddWithTrendlineTypeStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            sheet.Cells["A1"].PutValue("X Values");
            sheet.Cells["B1"].PutValue("Y Values");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue(i);
                sheet.Cells["B" + i].PutValue(i * 2);
            }

            // Diagramm erstellen
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Serie hinzufügen und Daten setzen
            chart.NSeries.Add("B2:B10", true);
            chart.NSeries[0].XValues = "A2:A10";
            chart.NSeries[0].Name = "Data Series";

            // Trendline mit TrendlineType und Name hinzufügen
            chart.NSeries[0].TrendLines.Add(TrendlineType.Logarithmic, "Logarithmic Trend");
            
            // Einige Trendline-Eigenschaften festlegen
            Trendline trendline = chart.NSeries[0].TrendLines[0];
            trendline.DisplayEquation = true;
            trendline.DisplayRSquared = true;
            
            workbook.Save("TrendlineDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [TrendlineType](../../trendlinetype/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


