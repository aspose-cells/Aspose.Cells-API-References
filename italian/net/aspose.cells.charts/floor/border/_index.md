---
title: "Floor.Border"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Floor. Ottiene o imposta la Line del bordo"
type: docs
url: /it/net/aspose.cells.charts/floor/border/
---
## Floor.Border property

Ottiene o imposta il bordo [`Line`](../../../aspose.cells.drawing/line/).

```csharp
public Line Border { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FloorPropertyBorderDemo
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

            // Aggiungi un grafico a colonne 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni il Floor del grafico
            Floor floor = chart.Floor;

            // Imposta le proprietà del bordo modificando il bordo esistente anziché crearne uno nuovo
            floor.Border.Color = Color.Red;
            floor.Border.Weight = WeightType.MediumLine;
            floor.Border.DashType = MsoLineDashStyle.DashDot;
            floor.Border.IsVisible = true;
            floor.Border.Transparency = 0.5;

            // Salva la cartella di lavoro
            workbook.Save("FloorBorderDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Line](../../../aspose.cells.drawing/line/)
* class [Floor](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


