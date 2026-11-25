---
title: "Chart.PivotSource"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. L'origine è il dato della tabella pivot. Se PivotSource non è vuoto il grafico è un PivotChart"
type: docs
url: /it/net/aspose.cells.charts/chart/pivotsource/
---
## Chart.PivotSource property

L'origine è i dati della tabella pivot. Se PivotSource non è vuoto, il grafico è un PivotChart.

```csharp
public string PivotSource { get; set; }
```

### Osservazioni

Se la tabella pivot "PivotTable1" nel foglio di lavoro "Sheet1" nel file "Book1.xls". Il pivotSource potrebbe essere "[Book1.xls]Sheet1!PivotTable1" se il grafico e la PivotTable non sono nella stessa cartella di lavoro. Se imposti questa proprietà, l'impostazione dell'origine dati precedente verrà persa.

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPivotSourceDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per la tabella pivot
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;
            
            // Aggiungi tabella pivot
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta l'origine pivot per il grafico
            chart.PivotSource = "Sheet1!PivotTable1";
            
            // Aggiorna i dati pivot e il grafico
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            chart.RefreshPivotData();
            
            // Salva la cartella di lavoro
            workbook.Save("PivotSourceDemo.xlsx", SaveFormat.Xlsx);
            
            Console.WriteLine("Chart PivotSource demo executed successfully.");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


