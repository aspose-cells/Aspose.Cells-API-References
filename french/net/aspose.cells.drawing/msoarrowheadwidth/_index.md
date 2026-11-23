---
title: "Énum MsoArrowheadWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Énum Aspose.Cells.Drawing.MsoArrowheadWidth. Énumère la largeur de l'extrémité de ligne du bord de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/msoarrowheadwidth/
---
## MsoArrowheadWidth enumeration

Énumère la largeur de l’extrémité de ligne de la bordure de forme.

```csharp
public enum MsoArrowheadWidth
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Narrow | `0` | Largeur d'extrémité de ligne courte. |
| Medium | `1` | Largeur d'extrémité de ligne moyenne. |
| Wide | `2` | Largeur d'extrémité de ligne large. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class MsoArrowheadWidthDemo
    {
        public static void MsoArrowheadWidthExample()
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

            // Créer une forme de ligne pour le graphique
            Line line = chart.Line;

            // Définir les styles et les largeurs des pointes de flèche
            line.BeginType = MsoArrowheadStyle.Arrow;
            line.BeginArrowWidth = MsoArrowheadWidth.Wide;
            line.EndType = MsoArrowheadStyle.Arrow;
            line.EndArrowWidth = MsoArrowheadWidth.Narrow;

            // Afficher les styles et les largeurs des pointes de flèche
            Console.WriteLine("Begin Arrowhead Width: " + line.BeginArrowWidth);
            Console.WriteLine("End Arrowhead Width: " + line.EndArrowWidth);

            // Enregistrez le classeur
            workbook.Save("MsoArrowheadWidthExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


