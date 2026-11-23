---
title: "Enum GradientStyleType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.GradientStyleType enum. Représente le style de dégradé d'ombrage"
type: docs
url: /fr/net/aspose.cells.drawing/gradientstyletype/
---
## GradientStyleType enumeration

Représente le style d’ombrage du dégradé.

```csharp
public enum GradientStyleType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| DiagonalDown | `0` | Style d’ombrage diagonal descendant |
| DiagonalUp | `1` | Style d’ombrage diagonal ascendant |
| FromCenter | `2` | Style d’ombrage à partir du centre |
| FromCorner | `3` | Style d’ombrage à partir du coin |
| Horizontal | `4` | Style d’ombrage horizontal |
| Vertical | `5` | Style d’ombrage vertical |
| Unknown | `6` | Style d’ombrage inconnu. Seulement pour le style d’ombrage (qui ne correspond à aucun membre de GradientStyleType) dans le fichier modèle. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientStyleTypeDemo
    {
        public static void GradientStyleTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Accéder à la zone de tracé du graphique
            PlotArea plotArea = chart.PlotArea;

            // Accéder au format de remplissage de la zone de tracé
            FillFormat fillFormat = plotArea.Area.FillFormat;

            // Définir un remplissage en dégradé bicolore avec le style DiagonalDown
            fillFormat.SetTwoColorGradient(Color.Blue, Color.White, GradientStyleType.DiagonalDown, 1);

            // Afficher le style de dégradé utilisé
            Console.WriteLine("Gradient Style: " + fillFormat.GradientStyle);

            // Enregistrez le classeur
            workbook.Save("GradientStyleTypeExample.xlsx");
            workbook.Save("GradientStyleTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


