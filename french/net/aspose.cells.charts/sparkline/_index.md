---
title: "Classe Sparkline"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.Sparkline class. Un sparkline représente un petit graphique ou une image dans une cellule de feuille de calcul qui fournit une représentation visuelle des données"
type: docs
url: /fr/net/aspose.cells.charts/sparkline/
---
## Sparkline class

Une sparkline représente un petit graphique ou une image dans une cellule de feuille de calcul qui fournit une représentation visuelle des données.

```csharp
public class Sparkline
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Column](../../aspose.cells.charts/sparkline/column/) { get; } | Obtient l'indice de colonne du sparkline. |
| [DataRange](../../aspose.cells.charts/sparkline/datarange/) { get; set; } | Représente la plage de données du sparkline. |
| [Row](../../aspose.cells.charts/sparkline/row/) { get; } | Obtient l'indice de ligne du sparkline. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage)(ImageOrPrintOptions) | Convertit un sparkline en image. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_1)(Stream, ImageOrPrintOptions) | Convertit un sparkline en image. |
| [ToImage](../../aspose.cells.charts/sparkline/toimage/#toimage_2)(string, ImageOrPrintOptions) | Convertit un sparkline en image. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SparklineDemo
    {
        public static void SparklineExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Définit la CellArea pour le sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Ajoute un groupe de sparklines à la feuille de calcul
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Ajouter un sparkline au groupe
            idx = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);
            Sparkline line = group.Sparklines[idx];

            // Afficher les détails du sparkline
            Console.WriteLine("Sparkline data range: " + line.DataRange + ", row: " + line.Row + ", column: " + line.Column);

            // Enregistrer le sparkline en tant qu'image
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                ImageType = Aspose.Cells.Drawing.ImageType.Png,
                HorizontalResolution = 300,
                VerticalResolution = 300
            };
            line.ToImage("output.png", options);

            // Enregistrez le classeur
            workbook.Save("SparklineExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


