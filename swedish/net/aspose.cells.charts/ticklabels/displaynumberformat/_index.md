---
title: "TickLabels.DisplayNumberFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabels-egenskap. Hämtar och anger visningsformatet för tick-etiketter"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/displaynumberformat/
---
## TickLabels.DisplayNumberFormat property

Hämtar och anger visningsformatet för siffror för ticketiketterna.

```csharp
public string DisplayNumberFormat { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyDisplayNumberFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(DateTime.Now);
            worksheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ange diagrammets dataområde
            chart.NSeries.Add("A2:A3", true);
            chart.NSeries.CategoryData = "B2:B3";
            
            // Ange talformat via NumberFormat-egenskapen istället
            chart.CategoryAxis.TickLabels.NumberFormat = "m/d/yyyy";
            chart.ValueAxis.TickLabels.NumberFormat = "#,##0";
            
            // Spara arbetsboken
            workbook.Save("TickLabelsDisplayNumberFormatDemo.xlsx");
            
            Console.WriteLine("DisplayNumberFormat for CategoryAxis: " + 
                chart.CategoryAxis.TickLabels.DisplayNumberFormat);
            Console.WriteLine("DisplayNumberFormat for ValueAxis: " + 
                chart.ValueAxis.TickLabels.DisplayNumberFormat);
        }
    }
}
```

### Se även

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


