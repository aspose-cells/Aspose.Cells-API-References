---
title: "ChartPoint.Area"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartPoint. Restituisce l'area"
type: docs
url: /it/net/aspose.cells.charts/chartpoint/area/
---
## ChartPoint.Area property

Restituisce l'`area`.

```csharp
public Area Area { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPointPropertyAreaDemo
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
            sheet.Cells["A5"].PutValue("D");
            
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["B5"].PutValue(40);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Accedi al primo punto nella prima serie e imposta le proprietà dell'area
            Aspose.Cells.Charts.ChartPoint point = chart.NSeries[0].Points[0];
            point.Area.ForegroundColor = System.Drawing.Color.Red;
            point.Area.FillFormat.Texture = TextureType.Granite;
            point.Area.Formatting = FormattingType.Custom;

            // Salva la cartella di lavoro
            workbook.Save("ChartPointAreaDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


