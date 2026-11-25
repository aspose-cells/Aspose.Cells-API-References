---
title: "Axis.IsAutoTickLabelSpacing"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Indica se la spaziatura delle etichette dei tick è automatica"
type: docs
url: /it/net/aspose.cells.charts/axis/isautoticklabelspacing/
---
## Axis.IsAutoTickLabelSpacing property

Indica se la spaziatura delle etichette dei segnapunti è automatica

```csharp
public bool IsAutoTickLabelSpacing { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsAutoTickLabelSpacingDemo
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

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configura l'asse dei valori
            Axis valueAxis = chart.ValueAxis;
            valueAxis.IsAutoTickLabelSpacing = true; // Core property demonstration
            
            // Configura l'asse delle categorie
            Axis categoryAxis = chart.CategoryAxis;
            categoryAxis.IsAutoTickLabelSpacing = false; // Core property demonstration
            categoryAxis.TickLabelSpacing = 2;

            workbook.Save("AxisPropertyIsAutoTickLabelSpacingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


