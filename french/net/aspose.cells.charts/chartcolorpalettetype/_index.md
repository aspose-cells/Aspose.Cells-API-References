---
title: "Enum ChartColorPaletteType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.ChartColorPaletteType enum. Enumère toutes les palettes monochromatiques utilisées dans un graphique Excel"
type: docs
url: /fr/net/aspose.cells.charts/chartcolorpalettetype/
---
## ChartColorPaletteType enumeration

Énumère toutes les palettes monochromatiques utilisées dans un graphique Excel.

```csharp
public enum ChartColorPaletteType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| MonochromaticPalette1 | `1` | dégradé de couleur de thème accent1, du sombre au clair. |
| MonochromaticPalette2 | `2` | dégradé de couleur de thème accent2, du sombre au clair. |
| MonochromaticPalette3 | `3` | dégradé de couleur de thème accent3, du sombre au clair. |
| MonochromaticPalette4 | `4` | dégradé de couleur de thème accent4, du sombre au clair. |
| MonochromaticPalette5 | `5` | dégradé de couleur de thème accent5, du sombre au clair. |
| MonochromaticPalette6 | `6` | dégradé de couleur de thème accent6, du sombre au clair. |
| MonochromaticPalette7 | `7` | dégradé de couleur de thème accent7. |
| MonochromaticPalette8 | `8` | dégradé de couleur de thème accent1, du clair au sombre. |
| MonochromaticPalette9 | `9` | dégradé de couleur de thème accent2, du clair au sombre. |
| MonochromaticPalette10 | `10` | dégradé de couleur de thème accent3, du clair au sombre. |
| MonochromaticPalette11 | `11` | dégradé de couleur de thème accent4, du clair au sombre. |
| MonochromaticPalette12 | `12` | dégradé de couleur de thème accent5, du clair au sombre. |
| MonochromaticPalette13 | `13` | dégradé de couleur de thème accent6, du clair au sombre. |

### Exemples

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
            // Créez un nouveau classeur pour la démonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Ajoutez un graphique d'exemple pour démontrer la palette de couleurs
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Démontrez l'utilisation de différentes valeurs d'énumération ChartColorPaletteType
                ChartColorPaletteType palette1 = ChartColorPaletteType.MonochromaticPalette1;
                ChartColorPaletteType palette5 = ChartColorPaletteType.MonochromaticPalette5;
                ChartColorPaletteType palette8 = ChartColorPaletteType.MonochromaticPalette8;

                // Afficher les valeurs d'énumération
                Console.WriteLine($"MonochromaticPalette1 value: {(int)palette1}");
                Console.WriteLine($"MonochromaticPalette5 value: {(int)palette5}");
                Console.WriteLine($"MonochromaticPalette8 value: {(int)palette8}");

                // Enregistrez le classeur
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

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


