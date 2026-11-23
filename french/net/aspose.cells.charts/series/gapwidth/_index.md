---
title: "Series.GapWidth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Retourne ou définit l'espace entre les groupes de barres ou de colonnes en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500"
type: docs
url: /fr/net/aspose.cells.charts/series/gapwidth/
---
## Series.GapWidth property

Renvoie ou définit l'espace entre les groupes de barres ou de colonnes, en pourcentage de la largeur de la barre ou de la colonne. La valeur de cette propriété doit être comprise entre 0 et 500.

```csharp
public short GapWidth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyGapWidthDemo
    {
        public static void Run()
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

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définissez la largeur de l'écart pour la première série
            chart.NSeries[0].GapWidth = 150;

            // Enregistrez le classeur
            workbook.Save("output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


