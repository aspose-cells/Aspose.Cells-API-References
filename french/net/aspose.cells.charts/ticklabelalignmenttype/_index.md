---
title: "Enum TickLabelAlignmentType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.TickLabelAlignmentType enum. Représente le type d'alignement du texte pour les étiquettes de graduation sur l'axe."
type: docs
url: /fr/net/aspose.cells.charts/ticklabelalignmenttype/
---
## TickLabelAlignmentType enumeration

Représente le type d'alignement du texte pour les étiquettes de graduation sur l'axe

```csharp
public enum TickLabelAlignmentType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Center | `0` | Spécifie que le texte est centré. |
| Left | `1` | Spécifie que le texte est aligné à gauche. |
| Right | `2` | Spécifie que le texte est aligné à droite.. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelAlignmentTypeDemo
    {
        public static void TickLabelAlignmentTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
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

            // Ajouter des séries au graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder aux étiquettes de graduation de l'axe des catégories
            TickLabels tickLabels = chart.CategoryAxis.TickLabels;

            // Définir le type d'alignement pour les étiquettes de graduation
            tickLabels.AlignmentType = TickLabelAlignmentType.Center;

            // Enregistrez le classeur
            workbook.Save("TickLabelAlignmentTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


