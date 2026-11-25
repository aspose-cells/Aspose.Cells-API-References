---
title: "Axis.CustomDisplayUnit"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Specifica un valore personalizzato per l'unità di visualizzazione"
type: docs
url: /it/net/aspose.cells.charts/axis/customdisplayunit/
---
## Axis.CustomDisplayUnit property

Specifica un valore personalizzato per l'unità di visualizzazione.

```csharp
public double CustomDisplayUnit { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCustomDisplayUnitDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10000000);
            worksheet.Cells["B3"].PutValue(20000000);
            worksheet.Cells["B4"].PutValue(30000000);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Imposta un'unità di visualizzazione personalizzata per l'asse dei valori
            chart.ValueAxis.CustomDisplayUnit = 1.0E7;
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Custom;
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


