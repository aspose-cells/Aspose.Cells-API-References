---
title: "Enumération LineJoinType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énumération Aspose.Cells.Drawing.LineJoinType. Représente les styles de jointure d'une ligne"
type: docs
url: /fr/net/aspose.cells.drawing/linejointype/
---
## LineJoinType enumeration

Représente les styles de jointure d’une ligne.

```csharp
public enum LineJoinType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Round | `0` | Jointure arrondie |
| Bevel | `1` | Jointure biseautée |
| Miter | `2` | Jointure en onglet |
| None | `3` | Aucune jointure |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LineJoinTypeDemo
    {
        public static void LineJoinTypeExample()
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

            // Accéder à l'axe de valeur principal
            Axis valueAxis = chart.ValueAxis;

            // Accéder au format de ligne des principales lignes de grille
            Line majorGridLines = valueAxis.MajorGridLines;

            // Définir le type de jointure de la ligne
            majorGridLines.JoinType = LineJoinType.Round;

            // Afficher le type de jointure
            Console.WriteLine("Line Join Type: " + majorGridLines.JoinType);

            // Enregistrez le classeur
            workbook.Save("LineJoinTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


