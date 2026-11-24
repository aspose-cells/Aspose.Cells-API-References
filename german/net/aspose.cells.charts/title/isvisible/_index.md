---
title: "Title.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Title-Eigenschaft. Gibt an, ob der Titel sichtbar ist"
type: docs
url: /de/net/aspose.cells.charts/title/isvisible/
---
## Title.IsVisible property

Stellt dar, ob der Titel sichtbar ist.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Füge ein Diagramm hinzu
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Demonstrieren Sie die IsVisible-Eigenschaft
            chart.Title.IsVisible = true;
            chart.Title.Text = "Sample Chart";
            chart.CategoryAxis.Title.IsVisible = true;
            chart.CategoryAxis.Title.Text = "Categories";
            chart.ValueAxis.Title.IsVisible = true;
            chart.ValueAxis.Title.Text = "Values";

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


