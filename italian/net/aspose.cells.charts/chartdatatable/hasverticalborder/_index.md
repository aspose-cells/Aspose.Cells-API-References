---
title: "ChartDataTable.HasVerticalBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartDataTable. True se la tabella dati del grafico ha bordi verticali delle celle"
type: docs
url: /it/net/aspose.cells.charts/chartdatatable/hasverticalborder/
---
## ChartDataTable.HasVerticalBorder property

Vero se la tabella dati del grafico ha bordi verticali delle celle

```csharp
public bool HasVerticalBorder { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasVerticalBorderDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Mostra tabella dati
            chart.ShowDataTable = true;
            
            // Accedi alla tabella dati tramite la proprietà ChartDataTable
            ChartDataTable dataTable = chart.ChartDataTable;

            // Dimostra la proprietà HasVerticalBorder
            Console.WriteLine("Initial HasVerticalBorder value: " + dataTable.HasVerticalBorder);
            
            // Attiva/disattiva bordi verticali
            dataTable.HasVerticalBorder = true;
            Console.WriteLine("After setting HasVerticalBorder to true: " + dataTable.HasVerticalBorder);
            
            dataTable.HasVerticalBorder = false;
            Console.WriteLine("After setting HasVerticalBorder to false: " + dataTable.HasVerticalBorder);

            // Salva la cartella di lavoro
            workbook.Save("ChartDataTable_HasVerticalBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


