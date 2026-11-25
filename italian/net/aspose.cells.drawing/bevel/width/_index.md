---
title: "Bevel.Width"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Bevel. Ottiene e imposta la larghezza del bevel o quanto profondamente viene applicato nella forma. In unità di punti"
type: docs
url: /it/net/aspose.cells.drawing/bevel/width/
---
## Bevel.Width property

Ottiene e imposta la larghezza della smussatura, o quanto nella forma viene applicata. In unità di punti.

```csharp
public double Width { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyWidthDemo
    {
        public static void Run()
        {
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

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la prima serie e imposta il formato 3D
            Series series = chart.NSeries[0];
            Format3D format3D = series.ShapeProperties.Format3D;
            
            // Configura le proprietà del bevel con la dimostrazione della larghezza
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 12; // Demonstrating Width property
            topBevel.Height = 6;

            // Salva la cartella di lavoro
            workbook.Save("BevelWidthDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


