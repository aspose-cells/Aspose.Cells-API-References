---
title: "Classe Area"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Drawing.Area class. Encapsule l'objet qui représente un format de zone"
type: docs
url: /fr/net/aspose.cells.drawing/area/
---
## Area class

Encapsule l'objet qui représente un format de zone.

```csharp
public class Area
```

## Propriétés

| Nom | Description |
| --- | --- |
| [BackgroundColor](../../aspose.cells.drawing/area/backgroundcolor/) { get; set; } | Obtient ou définit la couleur d'arrière-plan du `Area`. |
| [FillFormat](../../aspose.cells.drawing/area/fillformat/) { get; } | Représente un objet [`FillFormat`](./fillformat/) qui contient les propriétés de format de remplissage pour le graphique ou la forme spécifié. |
| [ForegroundColor](../../aspose.cells.drawing/area/foregroundcolor/) { get; set; } | Obtient ou définit la couleur de premier plan. |
| [Formatting](../../aspose.cells.drawing/area/formatting/) { get; set; } | Représente le formatage de la zone. |
| [InvertIfNegative](../../aspose.cells.drawing/area/invertifnegative/) { get; set; } | Si la propriété est vraie et que la valeur du point du graphique est un nombre négatif, la couleur de premier plan et la couleur d'arrière-plan seront échangées. |
| [Transparency](../../aspose.cells.drawing/area/transparency/) { get; set; } | Renvoie ou définit le degré de transparence de la zone comme une valeur de 0,0 (opaque) à 1,0 (transparent). |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class AreaDemo
    {
        public static void AreaExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            // Ajout d'une nouvelle feuille de calcul à l'objet Workbook
            int sheetIndex = workbook.Worksheets.Add();
            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Ajout de valeurs d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(-100);
            worksheet.Cells["A3"].PutValue(150);
            // Ajout d'un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Area, 5, 0, 15, 5);
            // Accès à l'instance du graphique nouvellement ajouté
            Chart chart = worksheet.Charts[chartIndex];
            // Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "A3"
            chart.NSeries.Add("A1:A3", true);

            // Accès à la zone du premier NSeries
            Area area = chart.NSeries[0].Area;

            // Définition des propriétés
            area.InvertIfNegative = true;
            area.ForegroundColor = Color.Red;
            area.BackgroundColor = Color.Yellow;
            area.Formatting = Aspose.Cells.Charts.FormattingType.Custom;
            area.Transparency = 0.5;

            // Enregistrement du fichier Excel
            workbook.Save("AreaExample.xlsx");
            workbook.Save("AreaExample.pdf");

        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


