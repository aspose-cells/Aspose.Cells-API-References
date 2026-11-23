---
title: "Enum ChartTextDirectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.ChartTextDirectionType enum. Représente le type de direction du texte du graphique"
type: docs
url: /fr/net/aspose.cells.charts/charttextdirectiontype/
---
## ChartTextDirectionType enumeration

Représente le type de direction du texte du graphique.

```csharp
public enum ChartTextDirectionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Horizontal | `0` | Type de direction horizontale. |
| Vertical | `1` | Type de direction verticale. |
| Rotate90 | `2` | Faire pivoter d'un angle de quatre-vingt-dix degrés. |
| Rotate270 | `3` | Faire pivoter d'un angle de 270 degrés. |
| Stacked | `4` | Texte empilé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartTextDirectionTypeDemo
    {
        public static void ChartTextDirectionTypeExample()
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
            
            // Ajouter une série de données au graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Définir le titre du graphique
            chart.Title.Text = "Sample Chart";
            chart.Title.Font.Color = Color.Blue;
            
            // Définir la direction du texte du titre du graphique
            chart.Title.DirectionType = ChartTextDirectionType.Rotate90;
            
            // Définir la direction du texte du titre de l'axe des catégories
            chart.CategoryAxis.Title.Text = "Categories";
            chart.CategoryAxis.Title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Définir la direction du texte du titre de l'axe des valeurs
            chart.ValueAxis.Title.Text = "Values";
            chart.ValueAxis.Title.DirectionType = ChartTextDirectionType.Horizontal;
            
            // Enregistrez le classeur
            workbook.Save("ChartTextDirectionTypeExample.xlsx");
            workbook.Save("ChartTextDirectionTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


