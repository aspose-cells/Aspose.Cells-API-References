---
title: "Chart.SwitchRowColumn"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Scambia riga/colonna"
type: docs
url: /it/net/aspose.cells.charts/chart/switchrowcolumn/
---
## Chart.SwitchRowColumn method

Scambia riga/colonna.

```csharp
public bool SwitchRowColumn()
```

### Valore di ritorno

False indica che lo scambio riga/colonna fallisce.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodSwitchRowColumnDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["A3"].PutValue("Item 2");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["A4"].PutValue("Item 3");
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C4"].PutValue(350);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.SetChartDataRange("A1:C4", true);
            
            // Mostra i valori originali delle serie
            Console.WriteLine("Before SwitchRowColumn:");
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            
            // Scambia riga/colonna
            chart.SwitchRowColumn();
            
            // Mostra i valori delle serie dopo il cambio
            Console.WriteLine("\nAfter SwitchRowColumn:");
            Console.WriteLine("Series 1 Values: " + chart.NSeries[0].Values);
            
            // Salva la cartella di lavoro
            workbook.Save("SwitchRowColumnDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


