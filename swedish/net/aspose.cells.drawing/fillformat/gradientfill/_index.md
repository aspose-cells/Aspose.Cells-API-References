---
title: "FillFormat.GradientFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Hämtar GradientFill-objekt"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/gradientfill/
---
## FillFormat.GradientFill property

Hämtar `GradientFill`-objekt.

```csharp
public GradientFill GradientFill { get; }
```

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientFillDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Tillhandahåll lite data för ett diagram
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Lägg till ett stapeldiagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            try
            {
                // Åtkomst till fyllningsformatet för det första serierområdet
                FillFormat fillFormat = chart.NSeries[0].Area.FillFormat;

                // Applicera en tvåfärgsgradient på serien
                fillFormat.SetTwoColorGradient(Color.Red, Color.Blue,
                                               GradientStyleType.Horizontal, 2);

                // Hämta GradientFill-objektet (skrivskyddad egenskap)
                GradientFill gradientFill = fillFormat.GradientFill;

                // Visa viss information om gradientfyllningen
                Console.WriteLine("GradientFill details:");
                Console.WriteLine($"  FillType      : {gradientFill.FillType}");
                Console.WriteLine($"  DirectionType: {gradientFill.DirectionType}");
                Console.WriteLine($"  Angle         : {gradientFill.Angle}");

                // Modifiera eventuellt gradientvinkeln med set-åtkomstmetoden
                gradientFill.Angle = 45.0f;
                Console.WriteLine($"  New Angle set to: {gradientFill.Angle}");

                // Spara arbetsboken
                workbook.Save("FillFormatGradientFillDemo.xlsx");
                Console.WriteLine("Workbook saved as FillFormatGradientFillDemo.xlsx");
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
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


