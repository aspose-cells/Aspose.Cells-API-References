---
title: "Chart.CategoryAxis"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Chart-Eigenschaft. Gibt die X‑Achse des Diagramms zurück"
type: docs
url: /de/net/aspose.cells.charts/chart/categoryaxis/
---
## Chart.CategoryAxis property

Liefert die X‑Achse des Diagramms.

```csharp
public Axis CategoryAxis { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyCategoryAxisDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Beispieldaten für das Diagramm hinzufügen
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ein Säulendiagramm hinzufügen
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Diagrammdatenbereich festlegen
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Auf CategoryAxis‑Eigenschaften zugreifen und sie ändern
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;
            chart.CategoryAxis.Title.Text = "Sample Categories";
            chart.CategoryAxis.Title.Font.Size = 12;

            // Speichere die Arbeitsmappe
            workbook.Save("CategoryAxisDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


