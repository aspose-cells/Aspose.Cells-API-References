---
title: "Area.BackgroundColor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Area. Ottiene o imposta il Color di sfondo dell'Area"
type: docs
url: /it/net/aspose.cells.drawing/area/backgroundcolor/
---
## Area.BackgroundColor property

Ottiene o imposta il Color di sfondo del [`Area`](../).

```csharp
public Color BackgroundColor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class AreaPropertyBackgroundColorDemo
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
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Imposta il colore di sfondo per l'area dell'asse di categoria
            chart.CategoryAxis.Area.BackgroundColor = System.Drawing.Color.Red;

            // Visualizza il colore di sfondo
            Console.WriteLine("Category Axis Background Color: " + chart.CategoryAxis.Area.BackgroundColor);

            // Salva la cartella di lavoro
            workbook.Save("AreaPropertyBackgroundColorDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


