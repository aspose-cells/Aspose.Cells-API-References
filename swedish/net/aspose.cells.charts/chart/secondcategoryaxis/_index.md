---
title: "Chart.SecondCategoryAxis"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Chart egenskap. Hämtar diagrammets andra X-axel"
type: docs
url: /sv/net/aspose.cells.charts/chart/secondcategoryaxis/
---
## Chart.SecondCategoryAxis property

Hämtar diagrammets andra X‑axel.

```csharp
public Axis SecondCategoryAxis { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySecondCategoryAxisDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Lägg till ett diagram med sekundär axel
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Lägg till serier i diagrammet
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aktivera sekundär kategori-axel
            chart.SecondCategoryAxis.IsVisible = true;
            chart.SecondCategoryAxis.Title.Text = "Secondary Category Axis";
            
            // Ställ in några egenskaper för den sekundära kategori-axeln
            chart.SecondCategoryAxis.MajorTickMark = TickMarkType.Cross;
            chart.SecondCategoryAxis.MinorTickMark = TickMarkType.Outside;
            chart.SecondCategoryAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;

            // Spara arbetsboken
            workbook.Save("SecondCategoryAxisDemo.xlsx");
        }
    }
}
```

### Se även

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


