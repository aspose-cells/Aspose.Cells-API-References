---
title: "Chart.ShowDataTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene o imposta un valore che indica se il grafico visualizza una tabella dei dati"
type: docs
url: /it/net/aspose.cells.charts/chart/showdatatable/
---
## Chart.ShowDataTable property

Ottiene o imposta un valore che indica se il grafico visualizza una tabella dati.

```csharp
public bool ShowDataTable { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyShowDataTableDemo
    {
        public static void Run()
        {
            // Crea una nuova Workbook
            Workbook workbook = new Workbook();
            Worksheet dataSheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            dataSheet.Cells["B1"].PutValue("Column 1");
            dataSheet.Cells["C1"].PutValue("Column 2");
            dataSheet.Cells["A2"].PutValue("Item 1");
            dataSheet.Cells["A3"].PutValue("Item 2");
            dataSheet.Cells["A4"].PutValue("Item 3");
            
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["B4"].PutValue(30);
            dataSheet.Cells["C2"].PutValue(15);
            dataSheet.Cells["C3"].PutValue(25);
            dataSheet.Cells["C4"].PutValue(35);

            // Aggiungi foglio grafico
            int chartIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartIndex];
            
            // Crea grafico
            chartSheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 1, 20, 10);
            Aspose.Cells.Charts.Chart chart = chartSheet.Charts[0];
            
            // Imposta la fonte dati
            chart.NSeries.Add("Sheet1!B2:C4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";
            
            // Abilita la visualizzazione della tabella dei dati
            chart.ShowDataTable = true;
            
            // Salva la cartella di lavoro
            workbook.Save("ChartWithDataTable.xlsx");
        }
    }
}
```

### Vedi anche

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


