---
title: "FillFormat.SetPresetColorGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-metod. Anger den specificerade fyllningen till en förinställd färggradient. Gäller endast för Excel 2007"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/setpresetcolorgradient/
---
## FillFormat.SetPresetColorGradient method

Ställer in den angivna fyllningen till en förinställd färggradient. Gäller endast för Excel 2007.

```csharp
public void SetPresetColorGradient(GradientPresetType presetColor, GradientStyleType style, 
    int variant)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| presetColor | GradientPresetType | Förinställd färgtyp |
| style | GradientStyleType | Gradientskuggningsstil. |
| variant | Int32 | Gradientvarianten. Kan vara ett värde från 1 till 4, motsvarande en av de fyra varianterna på fliken Gradient i dialogrutan Fylleffekter. Om stil är GradientStyle.FromCenter, kan Variant‑argumentet endast vara 1 eller 2. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetPresetColorGradientWithGradientPresetTypeGradientStylDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Item {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Skapa diagram
            int chartIndex = sheet.Charts.Add(ChartType.Column, 8, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Applicera gradientfyllning
            FillFormat fillFormat = chart.PlotArea.Area.FillFormat;
            fillFormat.SetPresetColorGradient(GradientPresetType.Daybreak, GradientStyleType.Vertical, 1);

            // Spara arbetsboken
            workbook.Save("SetPresetColorGradientDemo.xlsx");
        }
    }
}
```

### Se även

* enum [GradientPresetType](../../gradientpresettype/)
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


