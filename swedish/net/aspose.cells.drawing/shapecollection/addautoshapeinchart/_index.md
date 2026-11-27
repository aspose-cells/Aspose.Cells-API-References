---
title: "ShapeCollection.AddAutoShapeInChart"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeCollection-metod. Lägger till en AutoShape i diagrammet"
type: docs
url: /sv/net/aspose.cells.drawing/shapecollection/addautoshapeinchart/
---
## ShapeCollection.AddAutoShapeInChart method

Lägger till en AutoShape i diagrammet.

```csharp
public Shape AddAutoShapeInChart(AutoShapeType type, int top, int left, int height, int width)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | AutoShapeType | Auto shape-typ. |
| top | Int32 | Representerar den vertikala förskjutningen av textbox från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| vänster | Int32 | Representerar den vertikala förskjutningen av textbox från det övre vänstra hörnet i enheter av 1/4000 av diagramområdet. |
| höjd | Int32 | Representerar höjden på textbox, i enheter av 1/4000 av diagramområdet. |
| bredd | Int32 | Representerar bredden på textbox, i enheter av 1/4000 av diagramområdet. |

### Returvärde

Returnerar ett shape-objekt.

### Anmärkningar

Typen kunde inte vara Chart/Comment/Picture/OleObject/Polygon/DialogBox

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeCollectionMethodAddAutoShapeInChartWithAutoShapeTypeInt32Int32Int32InDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["B4"].PutValue(3000);

            // Lägg till ett diagram i kalkylbladet
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            try
            {
                // Anropa metoden AddAutoShapeInChart för att lägga till en stjärnform i diagrammet
                Shape shape = chart.Shapes.AddAutoShapeInChart(
                    AutoShapeType.Star16,  // AutoShapeType
                    100,                  // Top position (in pixels)
                    100,                  // Left position (in pixels)
                    200,                  // Height (in pixels)
                    200);                 // Width (in pixels)

                // Ställ in shape-egenskaper
                shape.Name = "SampleStar";
                shape.Fill.SolidFill.Color = System.Drawing.Color.Yellow;
                shape.Line.SolidFill.Color = System.Drawing.Color.Red;

                Console.WriteLine("Star shape added successfully to the chart.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AddAutoShapeInChart method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("ShapeCollectionMethodAddAutoShapeInChartDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../../shape/)
* enum [AutoShapeType](../../autoshapetype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


