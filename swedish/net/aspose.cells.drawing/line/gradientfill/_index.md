---
title: "Line.GradientFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Line-egenskap. Representerar gradientfyllning"
type: docs
url: /sv/net/aspose.cells.drawing/line/gradientfill/
---
## Line.GradientFill property

Representerar gradientfyllning.

```csharp
public GradientFill GradientFill { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;

    public class LinePropertyGradientFillDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för ett diagram
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Lägg till ett stapeldiagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Hämta den första punkten i den första serien
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];

            try
            {
                // Åtkomst till Line-objektet (kant) för punkten
                Line line = point.Border;

                // Läs GradientFill-egenskapen (skrivskyddad)
                GradientFill gradient = line.GradientFill;

                // Visa aktuella detaljer för gradientfyllning
                Console.WriteLine("Current GradientFill:");
                Console.WriteLine($"  FillType       = {gradient.FillType}");
                Console.WriteLine($"  DirectionType = {gradient.DirectionType}");
                Console.WriteLine($"  Angle          = {gradient.Angle}");

                // Modifiera gradienten med de tillhandahållna metoderna
                // Använd en typkonvertering till ett standard‑enum‑värde för att undvika att referera till en icke‑existerande medlem
                gradient.SetGradient(GradientFillType.Linear, 45.0, (GradientDirectionType)0);
                Console.WriteLine("GradientFill after SetGradient:");
                Console.WriteLine($"  Angle = {gradient.Angle}");

                // Spara arbetsboken
                workbook.Save("LinePropertyGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [GradientFill](../../gradientfill/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


