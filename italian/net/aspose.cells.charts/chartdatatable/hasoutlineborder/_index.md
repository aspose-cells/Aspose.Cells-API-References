---
title: "ChartDataTable.HasOutlineBorder"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartDataTable. True se la tabella dati del grafico ha bordi di contorno"
type: docs
url: /it/net/aspose.cells.charts/chartdatatable/hasoutlineborder/
---
## ChartDataTable.HasOutlineBorder property

Vero se la tabella dati del grafico ha bordi di contorno

```csharp
public bool HasOutlineBorder { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyHasOutlineBorderDemo
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

            // Mostra la tabella dati e ottieni l'oggetto ChartDataTable
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Dimostra la proprietà HasOutlineBorder
            dataTable.HasOutlineBorder = true; // Enable outline border
            Console.WriteLine("DataTable HasOutlineBorder: " + dataTable.HasOutlineBorder);

            // Salva la cartella di lavoro
            workbook.Save("ChartDataTableHasOutlineBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


