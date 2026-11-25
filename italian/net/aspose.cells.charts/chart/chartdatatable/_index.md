---
title: "Chart.ChartDataTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Rappresenta la tabella dati del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/chartdatatable/
---
## Chart.ChartDataTable property

Rappresenta la tabella dati del grafico.

```csharp
public ChartDataTable ChartDataTable { get; }
```

### Esempi

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyChartDataTableDemo
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
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta la fonte dati del grafico
            chart.NSeries.Add("=Sheet1!$B$2:$B$4", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$4";

            // Abilita e personalizza la tabella dati
            chart.ShowDataTable = true;
            ChartDataTable dataTable = chart.ChartDataTable;

            // Imposta le proprietà della tabella dati
            dataTable.ShowLegendKey = true;
            dataTable.HasBorderHorizontal = true;
            dataTable.HasBorderVertical = true;
            dataTable.HasBorderOutline = true;
            dataTable.AutoScaleFont = true;
            dataTable.BackgroundMode = BackgroundMode.Opaque;

            // Personalizza il carattere della tabella dati
            dataTable.Font.Name = "Arial";
            dataTable.Font.Size = 10;
            dataTable.Font.Color = Color.Blue;
            dataTable.Font.IsBold = true;

            // Personalizza i bordi della tabella dati
            dataTable.Border.Color = Color.Red;
            dataTable.Border.Style = LineType.Dash;
            dataTable.Border.Weight = WeightType.MediumLine;

            // Salva la cartella di lavoro
            workbook.Save("ChartDataTableDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartDataTable](../../chartdatatable/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


