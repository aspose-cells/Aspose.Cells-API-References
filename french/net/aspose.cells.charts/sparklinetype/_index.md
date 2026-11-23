---
title: "Enum SparklineType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.SparklineType enum. Représente les types de sparkline"
type: docs
url: /fr/net/aspose.cells.charts/sparklinetype/
---
## SparklineType enumeration

Représente les types de sparkline.

```csharp
public enum SparklineType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Line | `0` | Sparkline linéaire. |
| Column | `1` | Sparkline de colonne. |
| Stacked | `2` | Représente une sparkline Gain/Perte. |
| WinLoss | `2` | Représente une sparkline Gain/Perte. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineTypeDemo
    {
        public static void SparklineTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Définit la CellArea pour le sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Ajoute un groupe de sparklines à la feuille de calcul
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];

            // Ajoute des sparklines au groupe
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Personnalisez le groupe de sparkline
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;

            // Définissez les points hauts en vert et les points bas en rouge
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;

            // Définit le poids de la ligne
            group.LineWeight = 1.0;

            // Enregistrez le classeur
            workbook.Save("SparklineTypeExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


