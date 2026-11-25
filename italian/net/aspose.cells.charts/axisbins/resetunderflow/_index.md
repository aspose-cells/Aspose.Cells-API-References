---
title: "AxisBins.ResetUnderflow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo AxisBins. Ripristina l'underflow"
type: docs
url: /it/net/aspose.cells.charts/axisbins/resetunderflow/
---
## AxisBins.ResetUnderflow method

Ripristina l'underflow

```csharp
[Obsolete("This is an internal method.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ResetUnderflow()
```

### Osservazioni

NOTA: Questo metodo è ora obsoleto. È un metodo interno che non necessita di essere chiamato esternamente per evitare problemi. Questa proprietà sarà rimossa 12 mesi dopo, a partire da luglio 2024. Aspose si scusa per qualsiasi inconveniente tu possa aver riscontrato.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsMethodResetUnderflowDemo
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

            // Crea un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni l'asse dei valori
            Axis valueAxis = chart.ValueAxis;
            
            // Crea contenitori dell'asse
            valueAxis.Bins.IsAutomatic = false;
            valueAxis.Bins.Count = 5;
            valueAxis.Bins.Underflow = 5;
            
            try
            {
                // Chiama il metodo ResetUnderflow
                valueAxis.Bins.ResetUnderflow();
                
                Console.WriteLine("Underflow value after reset: " + valueAxis.Bins.Underflow);
                
                // Salva la cartella di lavoro
                workbook.Save("AxisBinsMethodResetUnderflowDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetUnderflow method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


