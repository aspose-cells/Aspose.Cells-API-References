---
title: "FillFormat.PresetColor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété FillFormat. Retourne la couleur de préréglage du dégradé pour le remplissage spécifié"
type: docs
url: /fr/net/aspose.cells.drawing/fillformat/presetcolor/
---
## FillFormat.PresetColor property

Renvoie la couleur prédéfinie du dégradé pour le remplissage spécifié.

```csharp
public GradientPresetType PresetColor { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyPresetColorDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Accédez au format de remplissage de la zone du graphique
            FillFormat fillFormat = chart.ChartArea.Area.FillFormat;

            // Définissez une couleur de préréglage de dégradé
            fillFormat.SetPresetColorGradient(GradientPresetType.Ocean, GradientStyleType.DiagonalUp, 2);

            // Affichez et vérifiez la couleur de préréglage
            Console.WriteLine("Preset Color: " + fillFormat.PresetColor);

            // Enregistrez le classeur
            workbook.Save("FillFormatPresetColorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [GradientPresetType](../../gradientpresettype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


