---
title: "Chart.RefreshPivotData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Chart. Aggiorna i dati del grafico dalla tabella pivot"
type: docs
url: /it/net/aspose.cells.charts/chart/refreshpivotdata/
---
## Chart.RefreshPivotData method

Aggiorna i dati del grafico dalla tabella pivot.

```csharp
public void RefreshPivotData()
```

### Osservazioni

Raccoglieremo i dati dalla fonte dati pivot al report della tabella pivot. Questo metodo è utilizzato solo per raccogliere tutti i dati in un grafico pivot.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartMethodRefreshPivotDataDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi dati di esempio al primo foglio di lavoro
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(100);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(200);
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B4"].PutValue(300);

            // Crea una tabella pivot
            Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
            pivotSheet.PivotTables.Add("A1", dataSheet.Cells["A1:B4"].Name, "PivotTable1");

            // Aggiungi un grafico
            int chartIndex = pivotSheet.Charts.Add(ChartType.Column, 5, 0, 15, 8);
            Aspose.Cells.Charts.Chart chart = pivotSheet.Charts[chartIndex];
            
            // Imposta origine dati del grafico pivot
            chart.PivotSource = "Pivot!PivotTable1";
            
            // Aggiorna i dati pivot nel grafico
            chart.RefreshPivotData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotChartWithRefresh.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


