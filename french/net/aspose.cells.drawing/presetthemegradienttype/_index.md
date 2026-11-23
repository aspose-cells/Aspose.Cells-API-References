---
title: "Énumération PresetThemeGradientType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.PresetThemeGradientType. Représente le type de dégradé de thème prédéfini"
type: docs
url: /fr/net/aspose.cells.drawing/presetthemegradienttype/
---
## PresetThemeGradientType enumeration

Représente le type de dégradé de thème prédéfini.

```csharp
public enum PresetThemeGradientType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| LightGradient | `0` | Dégradé clair |
| TopSpotlight | `1` | Spotlight supérieur |
| MediumGradient | `2` | Dégradé moyen |
| BottomSpotlight | `3` | Spotlight inférieur |
| RadialGradient | `4` | Dégradé radial |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetThemeGradientTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Category 1");
            worksheet.Cells["A3"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B3", true);

            // Appliquer le remplissage en dégradé à la première série
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = FillType.Gradient;
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                PresetThemeGradientType.RadialGradient, 
                ThemeColorType.Accent1);

            // Enregistrez le classeur
            workbook.Save("PresetThemeGradientDemo.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


