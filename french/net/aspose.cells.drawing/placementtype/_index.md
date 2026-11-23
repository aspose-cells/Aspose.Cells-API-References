---
title: "Enum PlacementType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.PlacementType. Représente la façon dont l'objet de dessin est attaché aux cellules en dessous."
type: docs
url: /fr/net/aspose.cells.drawing/placementtype/
---
## PlacementType enumeration

Représente la façon dont l’objet de dessin est attaché aux cellules en dessous.

```csharp
public enum PlacementType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| FreeFloating | `0` | Ne pas déplacer ni redimensionner avec les cellules. |
| Move | `1` | Déplacer mais ne pas redimensionner avec les cellules. |
| MoveAndSize | `2` | Déplacer et redimensionner avec les cellules. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class PlacementTypeDemo
    {
        public static void PlacementTypeExample()
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

            // Définir le type de placement du graphique
            chart.Placement = PlacementType.MoveAndSize;

            // Afficher le type de placement
            Console.WriteLine("Chart Placement Type: " + chart.Placement);

            // Enregistrez le classeur
            workbook.Save("PlacementTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


