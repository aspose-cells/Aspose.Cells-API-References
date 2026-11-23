---
title: "GradientFill.SetPresetThemeGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode GradientFill. Définit le remplissage de dégradé de thème prédéfini"
type: docs
url: /fr/net/aspose.cells.drawing/gradientfill/setpresetthemegradient/
---
## GradientFill.SetPresetThemeGradient method

Définit le remplissage en dégradé de thème prédéfini.

```csharp
public void SetPresetThemeGradient(PresetThemeGradientType gradientType, 
    ThemeColorType themeColorType)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| gradientType | PresetThemeGradientType | Le type de dégradé prédéfini. |
| themeColorType | ThemeColorType | Le type de couleur du thème. |

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillMethodSetPresetThemeGradientWithPresetThemeGradientTypeThemeCoDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);
            worksheet.Cells["A4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:A4", false);

            // Configurer le remplissage de la série avec un dégradé
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            series.Area.FillFormat.FillType = Aspose.Cells.Drawing.FillType.Gradient;
            
            // Démontrer SetPresetThemeGradient avec des paramètres spécifiés
            series.Area.FillFormat.GradientFill.SetPresetThemeGradient(
                Aspose.Cells.Drawing.PresetThemeGradientType.RadialGradient, 
                Aspose.Cells.ThemeColorType.Accent1);

            // Enregistrez le classeur
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [PresetThemeGradientType](../../presetthemegradienttype/)
* enum [ThemeColorType](../../../aspose.cells/themecolortype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


