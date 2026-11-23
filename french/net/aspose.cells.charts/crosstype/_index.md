---
title: "Enum CrossType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.CrossType enum. Représente le type de croisement d'axe"
type: docs
url: /fr/net/aspose.cells.charts/crosstype/
---
## CrossType enumeration

Représente le type d'intersection d'axe.

```csharp
public enum CrossType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Automatic | `0` | Microsoft Excel définit le point de croisement de l'axe. |
| Maximum | `1` | L'axe croise à la valeur maximale. |
| Minimum | `2` | L'axe croise à la valeur minimale. |
| Custom | `3` | L'axe croise à la valeur personnalisée. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class CrossTypeDemo
    {
        public static void CrossTypeExample()
        {
            // Instanciation d'un objet Workbook
            Workbook workbook = new Workbook();
            // Ajout d'une nouvelle feuille de calcul à l'objet Excel
            int sheetIndex = workbook.Worksheets.Add();
            // Obtention de la référence de la feuille de calcul nouvellement ajoutée en passant son indice de feuille
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            // Ajout de valeurs d'exemple aux cellules
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Ajout d'un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            // Accès à l'instance du graphique nouvellement ajouté
            Chart chart = worksheet.Charts[chartIndex];
            // Ajout de NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);

            // Définir la valeur maximale de l'axe des valeurs
            chart.ValueAxis.MaxValue = 200;
            // Définir la valeur minimale de l'axe des valeurs
            chart.ValueAxis.MinValue = 0;
            // Définir l'unité principale
            chart.ValueAxis.MajorUnit = 25;

            // L'axe Category(X) croise à la valeur maximale
            chart.ValueAxis.CrossType = CrossType.Maximum;

            // Définir le nombre de catégories ou de séries entre les étiquettes de repères
            chart.CategoryAxis.TickLabelSpacing = 2;

            // Enregistrement du fichier Excel
            workbook.Save("CrossTypeExample.xlsx");
            workbook.Save("CrossTypeExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


