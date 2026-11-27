---
title: "TickLabels.NumberFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TickLabels-egenskap. Representerar formatsträngen för TickLabels-objektet"
type: docs
url: /sv/net/aspose.cells.charts/ticklabels/numberformat/
---
## TickLabels.NumberFormat property

Representerar formatsträngen för TickLabels‑objektet.

```csharp
public string NumberFormat { get; set; }
```

### Anmärkningar

Formateringssträngen är densamma som en anpassad formatstränginställning i en cell. Till exempel, "$0".

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TickLabelsPropertyNumberFormatDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1.2345);
            worksheet.Cells["A3"].PutValue(2.3456);
            worksheet.Cells["A4"].PutValue(3.4567);

            // Skapa ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ange diagrammets dataområde
            chart.NSeries.Add("A2:A4", true);

            // Ange talformat för värdeaxelns tick-etiketter
            chart.ValueAxis.TickLabels.NumberFormat = "0.00";

            // Spara arbetsboken
            workbook.Save("TickLabelsNumberFormatDemo.xlsx");
        }
    }
}
```

### Se även

* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


