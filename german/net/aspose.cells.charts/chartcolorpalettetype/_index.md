---
title: "Enum ChartColorPaletteType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Charts.ChartColorPaletteType Enum. Enumeriert alle monochromen Paletten, die in einem Excel-Diagramm verwendet werden"
type: docs
url: /de/net/aspose.cells.charts/chartcolorpalettetype/
---
## ChartColorPaletteType enumeration

Enumeriert alle monochromen Paletten, die in einem Excel‑Diagramm verwendet werden.

```csharp
public enum ChartColorPaletteType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| MonochromaticPalette1 | `1` | Akzent1-Themenfarbverlauf, von dunkel nach hell. |
| MonochromaticPalette2 | `2` | Akzent2-Themenfarbverlauf, von dunkel nach hell. |
| MonochromaticPalette3 | `3` | Akzent3-Themenfarbverlauf, von dunkel nach hell. |
| MonochromaticPalette4 | `4` | Akzent4-Themenfarbverlauf, von dunkel nach hell. |
| MonochromaticPalette5 | `5` | Akzent5-Themenfarbverlauf, von dunkel nach hell. |
| MonochromaticPalette6 | `6` | Akzent6-Themenfarbverlauf, von dunkel nach hell. |
| MonochromaticPalette7 | `7` | Akzent7-Themenfarbverlauf. |
| MonochromaticPalette8 | `8` | Akzent1-Themenfarbverlauf, von hell nach dunkel. |
| MonochromaticPalette9 | `9` | Akzent2-Themenfarbverlauf, von hell nach dunkel. |
| MonochromaticPalette10 | `10` | Akzent3-Themenfarbverlauf, von hell nach dunkel. |
| MonochromaticPalette11 | `11` | Akzent4-Themenfarbverlauf, von hell nach dunkel. |
| MonochromaticPalette12 | `12` | Akzent5-Themenfarbverlauf, von hell nach dunkel. |
| MonochromaticPalette13 | `13` | Akzent6-Themenfarbverlauf, von hell nach dunkel. |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Fügen Sie ein Beispieldiagramm hinzu, um die Farbpalette zu demonstrieren
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Demonstrieren Sie die Verwendung verschiedener ChartColorPaletteType-Enum-Werte
                ChartColorPaletteType palette1 = ChartColorPaletteType.MonochromaticPalette1;
                ChartColorPaletteType palette5 = ChartColorPaletteType.MonochromaticPalette5;
                ChartColorPaletteType palette8 = ChartColorPaletteType.MonochromaticPalette8;

                // Die Enum-Werte anzeigen
                Console.WriteLine($"MonochromaticPalette1 value: {(int)palette1}");
                Console.WriteLine($"MonochromaticPalette5 value: {(int)palette5}");
                Console.WriteLine($"MonochromaticPalette8 value: {(int)palette8}");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


