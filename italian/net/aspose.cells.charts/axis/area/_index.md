---
title: "Axis.Area"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Axis. Ottiene l'Area"
type: docs
url: /it/net/aspose.cells.charts/axis/area/
---
## Axis.Area property

Ottiene l'`Area`.

```csharp
public Area Area { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class AxisPropertyAreaDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accedi alle proprietà dell'area dell'asse delle categorie
            chart.CategoryAxis.Area.BackgroundColor = Color.LightBlue;
            chart.CategoryAxis.Area.ForegroundColor = Color.White;
            chart.CategoryAxis.Area.Formatting = FormattingType.Custom;
            
            // Salva la cartella di lavoro
            workbook.Save("AxisPropertyAreaDemo_Output.xlsx");
            
            Console.WriteLine("Category Axis Area Background Color: " + chart.CategoryAxis.Area.BackgroundColor);
        }
    }
}
```

### Vedi anche

* class [Area](../../../aspose.cells.drawing/area/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


