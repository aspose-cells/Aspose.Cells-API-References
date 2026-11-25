---
title: "Chart.SecondCategoryAxis"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Ottiene il secondo asse X del grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/secondcategoryaxis/
---
## Chart.SecondCategoryAxis property

Ottiene il secondo asse X del grafico.

```csharp
public Axis SecondCategoryAxis { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySecondCategoryAxisDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(15);
            worksheet.Cells["C3"].PutValue(25);
            worksheet.Cells["C4"].PutValue(35);

            // Aggiungi un grafico con asse secondario
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi serie al grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Abilita l'asse di categoria secondario
            chart.SecondCategoryAxis.IsVisible = true;
            chart.SecondCategoryAxis.Title.Text = "Secondary Category Axis";
            
            // Imposta alcune proprietà dell'asse di categoria secondario
            chart.SecondCategoryAxis.MajorTickMark = TickMarkType.Cross;
            chart.SecondCategoryAxis.MinorTickMark = TickMarkType.Outside;
            chart.SecondCategoryAxis.TickLabelPosition = TickLabelPositionType.NextToAxis;

            // Salva la cartella di lavoro
            workbook.Save("SecondCategoryAxisDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


