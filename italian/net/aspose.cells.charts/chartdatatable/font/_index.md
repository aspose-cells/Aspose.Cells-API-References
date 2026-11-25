---
title: "ChartDataTable.Font"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartDataTable. Restituisce un oggetto Font che rappresenta l'impostazione del carattere della tabella dati del grafico specificato"
type: docs
url: /it/net/aspose.cells.charts/chartdatatable/font/
---
## ChartDataTable.Font property

Restituisce un oggetto `Font` che rappresenta l'impostazione del carattere della tabella dati del grafico specificato.

```csharp
public Font Font { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartDataTablePropertyFontDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Item");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(15);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Abilita tabella dati
            chart.ShowDataTable = true;
            
            // Ottieni l'oggetto della tabella dati
            ChartDataTable dataTable = chart.ChartDataTable;
            
            // Personalizza il carattere della tabella dati
            dataTable.Font.Size = 14;
            dataTable.Font.Color = Color.Red;
            dataTable.Font.IsBold = true;
            dataTable.Font.Name = "Arial";

            // Salva la cartella di lavoro
            workbook.Save("ChartDataTableFontDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Font](../../../aspose.cells/font/)
* class [ChartDataTable](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


