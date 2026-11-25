---
title: "SolidFill.Transparency"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SolidFill. Restituisce o imposta il grado di trasparenza dell'area come valore da 0.0 opaco a 1.0 chiaro."
type: docs
url: /it/net/aspose.cells.drawing/solidfill/transparency/
---
## SolidFill.Transparency property

Restituisce o imposta il grado di trasparenza dell'area come valore da 0,0 (opaco) a 1,0 (trasparente).

```csharp
public double Transparency { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SolidFillPropertyTransparencyDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi un grafico di esempio
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            chart.Calculate();

            // Aggiungi una forma per dimostrare la trasparenza
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                1000, 1000, 2000, 2000);
            
            // Imposta un riempimento solido con trasparenza.
            shape.Fill.SolidFill.Color = Color.Blue;
            shape.Fill.SolidFill.Transparency = 0.5; // 50% transparent

            // Aggiungi un'altra forma per il confronto (completamente opaca).
            Shape shape2 = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.FreeFloating, 
                3000, 1000, 2000, 2000);
            shape2.Fill.SolidFill.Color = Color.Blue;
            shape2.Fill.SolidFill.Transparency = 0; // 0% transparent (fully opaque)

            // Salva la cartella di lavoro
            workbook.Save("SolidFillTransparencyDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


