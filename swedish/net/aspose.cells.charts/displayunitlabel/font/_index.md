---
title: "DisplayUnitLabel.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DisplayUnitLabel egenskap. Hämtar ett Font-objekt av det specificerade ChartFrame-objektet"
type: docs
url: /sv/net/aspose.cells.charts/displayunitlabel/font/
---
## DisplayUnitLabel.Font property

Hämtar ett `Font`-objekt för det angivna ChartFrame-objektet.

```csharp
public override Font Font { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitLabelPropertyFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för diagrammet
            worksheet.Cells["A1"].PutValue(1000);
            worksheet.Cells["A2"].PutValue(2000);
            worksheet.Cells["A3"].PutValue(3000);
            worksheet.Cells["A4"].PutValue(4000);
            worksheet.Cells["A5"].PutValue(5000);

            // Lägg till ett diagram
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A5", true);

            // Ställ in displayenheter för värdeaxeln
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Thousands;
            chart.ValueAxis.DisplayUnitLabel.Text = "Thousands";

            // Hämta DisplayUnitLabel-instansen
            DisplayUnitLabel displayUnitLabel = chart.ValueAxis.DisplayUnitLabel;

            // Visa aktuella font-egenskaper
            Font currentFont = displayUnitLabel.Font;
            Console.WriteLine("Current Font Properties:");
            Console.WriteLine($"Name: {currentFont.Name}");
            Console.WriteLine($"Size: {currentFont.Size}");
            Console.WriteLine($"Color: {currentFont.Color}");
            Console.WriteLine($"Bold: {currentFont.IsBold}");
            Console.WriteLine($"Italic: {currentFont.IsItalic}");

            // Skapa en ny teckensnittsstil och tillämpa den på displayenhetsetiketten
            // Obs: Eftersom Font är skrivskyddad, modifierar vi dess egenskaper direkt
            currentFont.Name = "Arial";
            currentFont.Size = 12;
            currentFont.Color = System.Drawing.Color.Red;
            currentFont.IsBold = true;
            currentFont.IsItalic = false;
            currentFont.Underline = FontUnderlineType.Single;

            // Spara workbook för att se ändringarna
            workbook.Save("DisplayUnitLabelFontDemo.xlsx");
        }
    }
}
```

### Se även

* class [Font](../../../aspose.cells/font/)
* class [DisplayUnitLabel](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


