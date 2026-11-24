---
title: "DataLabels.ShowValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt das Anzeigeverhalten der Datenbeschriftungswerte eines bestimmten Diagramms an. True zeigt die Werte an. False blendet sie aus."
type: docs
url: /de/net/aspose.cells.charts/datalabels/showvalue/
---
## DataLabels.ShowValue property

Stellt das Anzeigeverhalten der Werte eines Datenlabels in einem bestimmten Diagramm dar. True zeigt die Werte an. False blendet sie aus.

```csharp
public bool ShowValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zum Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Diagrammdatenquelle festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen aktivieren und Werte anzeigen
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.Position = LabelPositionType.Center;

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsShowValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


