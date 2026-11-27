---
title: "Chart.CategoryAxis"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Hämtar diagrammets X-axel"
type: docs
url: /sv/net/aspose.cells.charts/chart/categoryaxis/
---
## Chart.CategoryAxis property

Hämtar diagrammets X‑axel.

```csharp
public Axis CategoryAxis { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett stapeldiagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Åtkomst till och ändra egenskaper för CategoryAxis
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;
            chart.CategoryAxis.Title.Text = "Sample Categories";
            chart.CategoryAxis.Title.Font.Size = 12;

            // Spara arbetsboken
            workbook.Save("CategoryAxisDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


