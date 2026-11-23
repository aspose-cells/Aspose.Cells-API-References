---
title: "Classe TickLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.TickLabels. Représente les étiquettes de repères associées aux repères sur un axe de graphique"
type: docs
url: /fr/net/aspose.cells.charts/ticklabels/
---
## TickLabels class

Représente les étiquettes de marques de graduation associées aux marques de graduation sur l'axe d'un graphique.

```csharp
public class TickLabels
```

## Propriétés

| Nom | Description |
| --- | --- |
| [AlignmentType](../../aspose.cells.charts/ticklabels/alignmenttype/) { get; set; } | Obtient et définit l'alignement du texte pour les étiquettes de repères sur l'axe. |
| [AutoScaleFont](../../aspose.cells.charts/ticklabels/autoscalefont/) { get; set; } | Vrai si le texte de l'objet change de taille de police lorsque la taille de l'objet change. La valeur par défaut est Vrai. |
| [BackgroundMode](../../aspose.cells.charts/ticklabels/backgroundmode/) { get; set; } | Obtient et définit le mode d'affichage de l'arrière-plan |
| [DirectionType](../../aspose.cells.charts/ticklabels/directiontype/) { get; set; } | Obtient et définit la direction du texte. |
| [DisplayNumberFormat](../../aspose.cells.charts/ticklabels/displaynumberformat/) { get; } | Obtient et définit le format numérique d'affichage des étiquettes de repères. |
| [Font](../../aspose.cells.charts/ticklabels/font/) { get; } | Renvoie un objet [`Font`](./font/) qui représente la police de l'objet TickLabels spécifié. |
| [IsAutomaticRotation](../../aspose.cells.charts/ticklabels/isautomaticrotation/) { get; set; } | Indique si l'angle de rotation est automatique |
| [Number](../../aspose.cells.charts/ticklabels/number/) { get; set; } | Représente le numéro de format pour l'objet TickLabels. |
| [NumberFormat](../../aspose.cells.charts/ticklabels/numberformat/) { get; set; } | Représente la chaîne de format pour l'objet TickLabels. |
| [NumberFormatLinked](../../aspose.cells.charts/ticklabels/numberformatlinked/) { get; set; } | Vrai si le format de nombre est lié aux cellules (de sorte que le format de nombre change dans les étiquettes lorsqu'il change dans les cellules). |
| [Offset](../../aspose.cells.charts/ticklabels/offset/) { get; set; } | Obtient et définit la distance des étiquettes par rapport à l'axe des catégories. Cela s'applique uniquement à l'axe des catégories (x). |
| [ReadingOrder](../../aspose.cells.charts/ticklabels/readingorder/) { get; set; } | Représente l'ordre de lecture du texte. |
| [RotationAngle](../../aspose.cells.charts/ticklabels/rotationangle/) { get; set; } | Représente l'angle de rotation du texte dans le sens des aiguilles d'une montre. |
| [TextDirection](../../aspose.cells.charts/ticklabels/textdirection/) { get; set; } | (**Obsolete.**) Représente l'ordre de lecture du texte. |
| [TickLabelItems](../../aspose.cells.charts/ticklabels/ticklabelitems/) { get; } | Obtient les étiquettes d'intervalle affichées de l'axe. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelsDemo
    {
        public static void TickLabelsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajoutez NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);

            // Accéder à l'axe des valeurs
            Axis valueAxis = chart.ValueAxis;

            // Accédez aux étiquettes d'intervalle de l'axe des valeurs
            TickLabels tickLabels = valueAxis.TickLabels;

            // Définissez les propriétés des étiquettes d'intervalle
            tickLabels.AutoScaleFont = true;
            tickLabels.BackgroundMode = BackgroundMode.Transparent;
            tickLabels.RotationAngle = 45;
            tickLabels.IsAutomaticRotation = false;
            tickLabels.NumberFormat = "0.00";
            tickLabels.Number = 2;
            tickLabels.NumberFormatLinked = true;
            tickLabels.Offset = 100;
            tickLabels.TextDirection = TextDirectionType.LeftToRight;
            tickLabels.ReadingOrder = TextDirectionType.LeftToRight;
            tickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Enregistrez le classeur
            workbook.Save("TickLabelsExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


