---
title: "Chart.CategoryAxis"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene l'asse X del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/categoryaxis/
---
## Chart.CategoryAxis property

Ottiene l'asse X del grafico.

```csharp
public Axis CategoryAxis { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyCategoryAxisDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico a colonne
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accedi e modifica le proprietà di CategoryAxis
            chart.CategoryAxis.CategoryType = CategoryType.CategoryScale;
            chart.CategoryAxis.Title.Text = "Sample Categories";
            chart.CategoryAxis.Title.Font.Size = 12;

            // Salva la cartella di lavoro
            workbook.Save("CategoryAxisDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


