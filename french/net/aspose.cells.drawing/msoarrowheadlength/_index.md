---
title: "Enum MsoArrowheadLength"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.MsoArrowheadLength. Énumère la largeur de l'extrémité de ligne du bord de la forme"
type: docs
url: /fr/net/aspose.cells.drawing/msoarrowheadlength/
---
## MsoArrowheadLength enumeration

Énumère la largeur de l’extrémité de ligne de la bordure de forme.

```csharp
public enum MsoArrowheadLength
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Short | `0` | Longueur d'extrémité de ligne courte |
| Medium | `1` | Longueur d'extrémité de ligne moyenne |
| Long | `2` | Longueur d'extrémité de ligne longue |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class MsoArrowheadLengthDemo
    {
        public static void MsoArrowheadLengthExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Créer une forme de ligne pour le graphique
            Line line = chart.Line;

            // Définir les longueurs des pointes de flèche
            line.BeginArrowLength = MsoArrowheadLength.Medium;
            line.EndArrowLength = MsoArrowheadLength.Long;

            // Afficher les longueurs des pointes de flèche
            Console.WriteLine("Begin Arrowhead Length: " + line.BeginArrowLength);
            Console.WriteLine("End Arrowhead Length: " + line.EndArrowLength);

            // Enregistrez le classeur
            workbook.Save("MsoArrowheadLengthExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


