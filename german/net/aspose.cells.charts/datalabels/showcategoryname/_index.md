---
title: "DataLabels.ShowCategoryName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DataLabels-Eigenschaft. Gibt das Anzeigeverhalten des Kategorienamens einer Diagrammdatenbeschriftung an. Wahr, um den Kategorienamen für die Datenbeschriftungen im Diagramm anzuzeigen. Falsch, um ihn zu verbergen."
type: docs
url: /de/net/aspose.cells.charts/datalabels/showcategoryname/
---
## DataLabels.ShowCategoryName property

Stellt das Anzeigeverhalten des Kategorienamens eines Datenlabels in einem bestimmten Diagramm dar. True zeigt den Kategorienamen für die Datenlabels im Diagramm an. False blendet ihn aus.

```csharp
public bool ShowCategoryName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowCategoryNameDemo
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

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Datenbeschriftungen aktivieren und Eigenschaften festlegen
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.ShowCategoryName = true;
            dataLabels.SeparatorType = DataLabelsSeparatorType.Semicolon;

            // Speichere die Arbeitsmappe
            workbook.Save("DataLabelsShowCategoryNameDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


