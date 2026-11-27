---
title: "Enum ChartColorPaletteType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Charts.ChartColorPaletteType‑enum. Enumererar alla monokroma paletter som används i ett Excel‑diagram"
type: docs
url: /sv/net/aspose.cells.charts/chartcolorpalettetype/
---
## ChartColorPaletteType enumeration

Enumererar alla monokroma paletter som används i ett Excel‑diagram.

```csharp
public enum ChartColorPaletteType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| MonochromaticPalette1 | `1` | accent1 temafärggradient, mörk till ljus. |
| MonochromaticPalette2 | `2` | accent2 temafärggradient, mörk till ljus. |
| MonochromaticPalette3 | `3` | accent3 temafärggradient, mörk till ljus. |
| MonochromaticPalette4 | `4` | accent4 temafärggradient, mörk till ljus. |
| MonochromaticPalette5 | `5` | accent5 temafärggradient, mörk till ljus. |
| MonochromaticPalette6 | `6` | accent6 temafärggradient, mörk till ljus. |
| MonochromaticPalette7 | `7` | accent7 temafärggradient. |
| MonochromaticPalette8 | `8` | accent1 temafärggradient, ljus till mörk. |
| MonochromaticPalette9 | `9` | accent2 temafärggradient, ljus till mörk. |
| MonochromaticPalette10 | `10` | accent3 temafärggradient, ljus till mörk. |
| MonochromaticPalette11 | `11` | accent4 temafärggradient, ljus till mörk. |
| MonochromaticPalette12 | `12` | accent5 temafärggradient, ljus till mörk. |
| MonochromaticPalette13 | `13` | accent6-temafärggradient, ljus till mörk. |

### Exempel

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
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till ett exempeldiagram för att demonstrera färgpaletten
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Demonstrera användning av olika värden för enum ChartColorPaletteType
                ChartColorPaletteType palette1 = ChartColorPaletteType.MonochromaticPalette1;
                ChartColorPaletteType palette5 = ChartColorPaletteType.MonochromaticPalette5;
                ChartColorPaletteType palette8 = ChartColorPaletteType.MonochromaticPalette8;

                // Visa enum‑värden
                Console.WriteLine($"MonochromaticPalette1 value: {(int)palette1}");
                Console.WriteLine($"MonochromaticPalette5 value: {(int)palette5}");
                Console.WriteLine($"MonochromaticPalette8 value: {(int)palette8}");

                // Spara arbetsboken
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

### Se även

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


