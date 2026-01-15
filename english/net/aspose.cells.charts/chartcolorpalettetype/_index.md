---
title: Enum ChartColorPaletteType
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Charts.ChartColorPaletteType enum. Enumerates all Monochromatic Palettes used in Excel chart
type: docs
url: /net/aspose.cells.charts/chartcolorpalettetype/
---
## ChartColorPaletteType enumeration

Enumerates all Monochromatic Palettes used in Excel chart.

```csharp
public enum ChartColorPaletteType
```

### Values

| Name | Value | Description |
| --- | --- | --- |
| MonochromaticPalette1 | `1` | accent1 theme color gradient, dark to light. |
| MonochromaticPalette2 | `2` | accent2 theme color gradient, dark to light. |
| MonochromaticPalette3 | `3` | accent3 theme color gradient, dark to light. |
| MonochromaticPalette4 | `4` | accent4 theme color gradient, dark to light. |
| MonochromaticPalette5 | `5` | accent5 theme color gradient, dark to light. |
| MonochromaticPalette6 | `6` | accent6 theme color gradient, dark to light. |
| MonochromaticPalette7 | `7` | accent7 theme color gradient. |
| MonochromaticPalette8 | `8` | accent1 theme color gradient, light to dark. |
| MonochromaticPalette9 | `9` | accent2 theme color gradient, light to dark. |
| MonochromaticPalette10 | `10` | accent3 theme color gradient, light to dark. |
| MonochromaticPalette11 | `11` | accent4 theme color gradient, light to dark. |
| MonochromaticPalette12 | `12` | accent5 theme color gradient, light to dark. |
| MonochromaticPalette13 | `13` | accent6 theme color gradient, light to dark. |

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartColorPaletteTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook for demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Add a sample chart to demonstrate the color palette
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Demonstrate using different ChartColorPaletteType enum values
                ChartColorPaletteType palette1 = ChartColorPaletteType.MonochromaticPalette1;
                ChartColorPaletteType palette5 = ChartColorPaletteType.MonochromaticPalette5;
                ChartColorPaletteType palette8 = ChartColorPaletteType.MonochromaticPalette8;

                // Display the enum values
                Console.WriteLine($"MonochromaticPalette1 value: {(int)palette1}");
                Console.WriteLine($"MonochromaticPalette5 value: {(int)palette5}");
                Console.WriteLine($"MonochromaticPalette8 value: {(int)palette8}");

                // Save the workbook
                workbook.Save("ChartColorPaletteTypeDemo.xlsx");
                Console.WriteLine("ChartColorPaletteType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ChartColorPaletteType: {ex.Message}");
            }
        }
    }
}
```

### See Also

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


