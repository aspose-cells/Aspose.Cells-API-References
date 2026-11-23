---
title: "FillFormat.SetPresetColorGradient"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Méthode FillFormat. Définit le remplissage spécifié sur un dégradé de couleur prédéfinie. S'applique uniquement à Excel 2007"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/setpresetcolorgradient/
---
## FillFormat.SetPresetColorGradient method

Définit le remplissage spécifié comme un dégradé à couleur prédéfinie. S'applique uniquement à Excel 2007.

```csharp
public void SetPresetColorGradient(GradientPresetType presetColor, GradientStyleType style, 
    int variant)
```

| Paramètre | Type | Description |
| --- | --- | --- |
| presetColor | GradientPresetType | Type de couleur prédéfinie |
| style | GradientStyleType | Style d’ombrage du dégradé. |
| variant | Int32 | La variante du dégradé. Peut être une valeur de 1 à 4, correspondant à l'une des quatre variantes de l'onglet Dégradé dans la boîte de dialogue Effets de remplissage. Si le style est GradientStyle.FromCenter, l'argument Variant ne peut être que 1 ou 2. |

### Exemples

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

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 5; i++)
            {
                sheet.Cells[$"A{i}"].PutValue($"Item {i-1}");
                sheet.Cells[$"B{i}"].PutValue(i * 10);
            }

            // Créer un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 8, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Appliquer un remplissage en dégradé
            FillFormat fillFormat = chart.PlotArea.Area.FillFormat;
            fillFormat.SetPresetColorGradient(GradientPresetType.Daybreak, GradientStyleType.Vertical, 1);

            // Enregistrez le classeur
            workbook.Save("SetPresetColorGradientDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientPresetType](../../gradientpresettype/)
* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


