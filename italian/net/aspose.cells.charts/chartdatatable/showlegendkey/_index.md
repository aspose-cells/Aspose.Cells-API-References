---
title: "ChartDataTable.ShowLegendKey"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartDataTable. True se la chiave della legenda dell'etichetta dati è visibile"
type: docs
url: /it/net/aspose.cells.charts/chartdatatable/showlegendkey/
---
## ChartDataTable.ShowLegendKey property

Vero se la chiave della legenda dell'etichetta dati è visibile.

```csharp
public bool ShowLegendKey { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyShowLegendKeyDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abilita la tabella dati con chiave della legenda
            chart.ShowDataTable = true;
            // Accedi a DataTable tramite le proprietà del Chart
            if (chart.ChartDataTable != null)
            {
                chart.ChartDataTable.ShowLegendKey = true;
            }

            // Salva la cartella di lavoro
            workbook.Save("ChartDataTableShowLegendKeyDemo.xlsx");

            Console.WriteLine("Chart created with ShowLegendKey enabled in data table.");
        }
    }
}
```

### Vedi anche

* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


