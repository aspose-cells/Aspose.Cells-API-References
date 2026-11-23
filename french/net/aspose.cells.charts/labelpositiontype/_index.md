---
title: "Enumération LabelPositionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Charts.LabelPositionType. Représente le type de position des étiquettes de données"
type: docs
url: /fr/net/aspose.cells.charts/labelpositiontype/
---
## LabelPositionType enumeration

Représente le type de position de l'étiquette de données.

```csharp
public enum LabelPositionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Center | `0` | S'applique uniquement aux graphiques à barres, 2D/3D en secteurs |
| InsideBase | `1` | S'applique uniquement aux graphiques à barres, 2D/3D en secteurs |
| InsideEnd | `2` | S'applique uniquement aux graphiques à barres |
| OutsideEnd | `3` | S'applique uniquement aux graphiques à barres, 2d/3d en secteurs |
| Above | `4` | S'applique uniquement aux graphiques en lignes |
| Below | `5` | S'applique uniquement aux graphiques en lignes |
| Left | `6` | S'applique uniquement aux graphiques en lignes |
| Right | `7` | S'applique uniquement aux graphiques en lignes |
| BestFit | `8` | S'applique uniquement aux graphiques en secteurs 2D/3D |
| Moved | `9` | L'utilisateur a déplacé les étiquettes de données. Ceci n'est destiné qu'à la lecture du graphique depuis le fichier modèle. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LabelPositionTypeDemo
    {
        public static void LabelPositionTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple pour le graphique
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

            // Ajoutez la série de données au graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accédez aux étiquettes de données de la première série
            DataLabels dataLabels = chart.NSeries[0].DataLabels;

            // Définir la position des étiquettes de données
            dataLabels.Position = LabelPositionType.InsideBase;

            // Afficher le nom de la catégorie dans les étiquettes de données
            dataLabels.ShowCategoryName = true;

            // Afficher la valeur dans les étiquettes de données
            dataLabels.ShowValue = true;

            // Enregistrez le classeur
            workbook.Save("LabelPositionTypeExample.xlsx");
            workbook.Save("LabelPositionTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


