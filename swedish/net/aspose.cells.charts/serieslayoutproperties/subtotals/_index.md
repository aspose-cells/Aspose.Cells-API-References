---
title: "SeriesLayoutProperties.Subtotals"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SeriesLayoutProperties-egenskap. Representerar indexet för en delsummapunkt"
type: docs
url: /sv/net/aspose.cells.charts/serieslayoutproperties/subtotals/
---
## SeriesLayoutProperties.Subtotals property

Representerar indexet för en delsumme-datapunkt.

```csharp
public int[] Subtotals { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertySubtotalsDemo
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

            // Lägg till ett diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ställ in delsummor för den första serien
            chart.NSeries[0].LayoutProperties.Subtotals = new int[] { 0, 3 };

            // Verifiera att delsummor har ställts in korrekt
            Console.WriteLine("Subtotal at index 0: " + chart.NSeries[0].LayoutProperties.Subtotals[0]);
            Console.WriteLine("Subtotal at index 1: " + chart.NSeries[0].LayoutProperties.Subtotals[1]);

            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


