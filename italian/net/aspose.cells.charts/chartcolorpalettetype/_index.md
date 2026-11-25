---
title: "Enum ChartColorPaletteType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Charts.ChartColorPaletteType enum. Elenca tutte le palette monocromatiche utilizzate in un grafico Excel"
type: docs
url: /it/net/aspose.cells.charts/chartcolorpalettetype/
---
## ChartColorPaletteType enumeration

Elenca tutte le palette monocromatiche utilizzate in un grafico Excel.

```csharp
public enum ChartColorPaletteType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| MonochromaticPalette1 | `1` | gradiente di colore tema accent1, da scuro a chiaro. |
| MonochromaticPalette2 | `2` | gradiente di colore del tema accent2, da scuro a chiaro. |
| MonochromaticPalette3 | `3` | gradiente di colore del tema accent3, da scuro a chiaro. |
| MonochromaticPalette4 | `4` | gradiente di colore del tema accent4, da scuro a chiaro. |
| MonochromaticPalette5 | `5` | gradiente di colore del tema accent5, da scuro a chiaro. |
| MonochromaticPalette6 | `6` | gradiente di colore del tema accent6, da scuro a chiaro. |
| MonochromaticPalette7 | `7` | gradiente di colore del tema accent7. |
| MonochromaticPalette8 | `8` | gradiente di colore del tema accent1, da chiaro a scuro. |
| MonochromaticPalette9 | `9` | gradiente di colore del tema accent2, da chiaro a scuro. |
| MonochromaticPalette10 | `10` | gradiente di colore del tema accent3, da chiaro a scuro. |
| MonochromaticPalette11 | `11` | gradiente di colore del tema accent4, da chiaro a scuro. |
| MonochromaticPalette12 | `12` | gradiente di colore del tema accent5, da chiaro a scuro. |
| MonochromaticPalette13 | `13` | gradiente di colore del tema accent6, da chiaro a scuro. |

### Esempi

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
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi un grafico di esempio per dimostrare la palette di colori
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Dimostra l'uso di diversi valori dell'enumerazione ChartColorPaletteType
                ChartColorPaletteType palette1 = ChartColorPaletteType.MonochromaticPalette1;
                ChartColorPaletteType palette5 = ChartColorPaletteType.MonochromaticPalette5;
                ChartColorPaletteType palette8 = ChartColorPaletteType.MonochromaticPalette8;

                // Visualizzare i valori dell'enumerazione
                Console.WriteLine($"MonochromaticPalette1 value: {(int)palette1}");
                Console.WriteLine($"MonochromaticPalette5 value: {(int)palette5}");
                Console.WriteLine($"MonochromaticPalette8 value: {(int)palette8}");

                // Salva la cartella di lavoro
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

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


