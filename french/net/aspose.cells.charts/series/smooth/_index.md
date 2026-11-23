---
title: "Series.Smooth"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété de Series. Représente le lissage de courbe. Vrai si le lissage de courbe est activé pour le graphique en ligne ou le nuage de points. S'applique uniquement aux graphiques en ligne et aux nuages de points avec lignes"
type: docs
url: /fr/net/aspose.cells.charts/series/smooth/
---
## Series.Smooth property

Représente le lissage de courbe. Vrai si le lissage de courbe est activé pour le graphique en lignes ou le nuage de points. S'applique uniquement aux graphiques en lignes et aux nuages de points avec lignes.

```csharp
public bool Smooth { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySmoothDemo
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

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir la propriété Smooth pour la première série
            chart.NSeries[0].Smooth = true;

            // Enregistrez le classeur
            workbook.Save("SmoothPropertyDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


