---
title: "ChartFrame.IsDefaultPosBeSet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartFrame. Indica se la posizione predefinita DefaultX DefaultY DefaultWidth e DefaultHeight è impostata"
type: docs
url: /it/net/aspose.cells.charts/chartframe/isdefaultposbeset/
---
## ChartFrame.IsDefaultPosBeSet property

Indica se la posizione predefinita (DefaultX, DefaultY, DefaultWidth e DefaultHeight) è impostata.

```csharp
public bool IsDefaultPosBeSet { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartFramePropertyIsDefaultPosBeSetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Bar, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi alle etichette dei dati
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            
            // Dimostra la proprietà IsDefaultPosBeSet
            Console.WriteLine("IsDefaultPosBeSet before setting position: " + dataLabels.IsDefaultPosBeSet);
            
            // Modifica la posizione e controlla nuovamente la proprietà
            dataLabels.Position = LabelPositionType.InsideBase;
            Console.WriteLine("IsDefaultPosBeSet after setting position: " + dataLabels.IsDefaultPosBeSet);
        }
    }
}
```

### Vedi anche

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


