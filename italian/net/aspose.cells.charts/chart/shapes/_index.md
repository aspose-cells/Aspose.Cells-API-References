---
title: "Chart.Shapes"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Chart. Restituisce tutte le forme di disegno in questo grafico"
type: docs
url: /it/net/aspose.cells.charts/chart/shapes/
---
## Chart.Shapes property

Restituisce tutte le forme di disegno in questo grafico.

```csharp
public ShapeCollection Shapes { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyShapesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per il grafico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico al foglio di lavoro
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta la fonte dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Aggiungi una forma al grafico
            Aspose.Cells.Drawing.Shape shape = chart.Shapes.AddShape(MsoDrawingType.TextBox, 1000, 1000, 2000, 1000, 0, 0);
            shape.Text = "Sample Shape";
            
            // Modifica le proprietà della forma
            shape.LeftInShape = 4000 - shape.WidthInShape;
            shape.TopInShape = 4000 - shape.HeightInShape;
            
            // Salva la cartella di lavoro
            workbook.Save("ChartPropertyShapesDemo_out.xlsx");
        }
    }
}
```

### Vedi anche

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


