---
title: "ShapeCollection.AddLabelInChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en etikett i diagrammet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addlabelinchart/
---
## ShapeCollection.AddLabelInChart method

Lägger till en label i diagrammet.

```csharp
public Label AddLabelInChart(int top, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| top | Int32 | Representerar den vertikala förskjutningen av etiketten från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| vänster | Int32 | Representerar den vertikala förskjutningen av etiketten från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| höjd | Int32 | Representerar etikettens höjd, i enheter av 1/4000 av diagramområdet. |
| bredd | Int32 | Representerar etikettens bredd, i enheter av 1/4000 av diagramområdet. |

### Returvärde

Ett nytt Label-objekt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att skapa ett diagram
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];            
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Anropa AddLabelInChart-metoden med parametrarna (top, left, height, width)
                Label label = chart.Shapes.AddLabelInChart(100, 100, 200, 200);
                
                // Ställ in etikettens egenskaper
                label.Text = "Sample Chart Label";
                label.Font.Color = System.Drawing.Color.Red;
                label.Font.Size = 12;

                Console.WriteLine("Label added successfully to chart with parameters (100, 100, 200, 50)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddLabelInChart method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("ShapeCollectionMethodAddLabelInChartWithInt32Int32Int32Int32Demo.xlsx");
        }
    }
}
```

### Se även

* class [Label](../../label/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


