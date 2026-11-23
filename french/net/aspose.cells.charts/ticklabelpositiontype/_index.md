---
title: "Enum TickLabelPositionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.TickLabelPositionType enum. Représente le type de position des étiquettes de repère sur l'axe spécifié"
type: docs
url: /fr/net/aspose.cells.charts/ticklabelpositiontype/
---
## TickLabelPositionType enumeration

Représente le type de position des étiquettes de graduation sur l'axe spécifié.

```csharp
public enum TickLabelPositionType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| High | `0` | Le type de position est haut. |
| Low | `1` | Le type de position est bas. |
| NextToAxis | `2` | Le type de position est à côté de l'axe. |
| None | `3` | Le type de position est aucun. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TickLabelPositionTypeDemo
    {
        public static void TickLabelPositionTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Ajoutez NSeries (source de données du graphique) au graphique allant de la cellule "A1" à "B3"
            chart.NSeries.Add("A1:B3", true);
            
            // Accédez à l'axe des catégories
            Axis categoryAxis = chart.CategoryAxis;
            
            // Définissez la position de l'étiquette de repère sur Haut
            categoryAxis.TickLabelPosition = TickLabelPositionType.High;
            
            // Enregistrez le classeur
            workbook.Save("TickLabelPositionTypeExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


