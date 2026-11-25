---
title: "Axis.CrossType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Rappresenta il CrossType sull'asse specificato dove l'altro asse lo attraversa"
type: docs
url: /it/net/aspose.cells.charts/axis/crosstype/
---
## Axis.CrossType property

Rappresenta il `CrossType` sull'asse specificato dove l'altro asse lo attraversa.

```csharp
public CrossType CrossType { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCrossTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Crea grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configura l'asse dei valori
            chart.ValueAxis.MaxValue = 200;
            chart.ValueAxis.MinValue = 0;
            chart.ValueAxis.MajorUnit = 25;
            
            // Dimostra la proprietà CrossType
            chart.ValueAxis.CrossType = CrossType.Maximum;

            workbook.Save("AxisPropertyCrossTypeDemo.xlsx");
        }
    }
}
```

### Vedi anche

* enum [CrossType](../../crosstype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


