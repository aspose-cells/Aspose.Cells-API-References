---
title: "SeriesLayoutProperties.QuartileCalculation"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SeriesLayoutProperties. Rappresenta le proprietà statistiche per la serie"
type: docs
url: /it/net/aspose.cells.charts/serieslayoutproperties/quartilecalculation/
---
## SeriesLayoutProperties.QuartileCalculation property

Rappresenta le proprietà statistiche per la serie.

```csharp
public QuartileCalculationType QuartileCalculation { get; set; }
```

### Osservazioni

Applicabile solo al grafico BoxWhisker.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyQuartileCalculationDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.BoxWhisker, 7, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            Aspose.Cells.Charts.SeriesLayoutProperties layoutProperties = chart.NSeries[0].LayoutProperties;
            layoutProperties.QuartileCalculation = Aspose.Cells.Charts.QuartileCalculationType.Exclusive;

            workbook.Save("QuartileCalculationDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [QuartileCalculationType](../../quartilecalculationtype/)
* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


