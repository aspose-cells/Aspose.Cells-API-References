---
title: "Series.Overlap"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Spécifie comment les barres et les colonnes sont positionnées. Peut être une valeur entre 100 et 100. S'applique uniquement aux graphiques à barres 2D et aux graphiques à colonnes 2D"
type: docs
url: /fr/net/aspose.cells.charts/series/overlap/
---
## Series.Overlap property

Spécifie comment les barres et colonnes sont positionnées. Peut être une valeur entre -100 et 100. S'applique uniquement aux graphiques à barres 2D et à colonnes 2D.

```csharp
public short Overlap { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyOverlapDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Series1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["C1"].PutValue("Series2");
            sheet.Cells["C2"].PutValue(15);
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["C4"].PutValue(35);

            // Ajoutez un graphique à colonnes groupées
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir la propriété de chevauchement pour la première série
            chart.NSeries[0].Overlap = -40;

            // Enregistrez le classeur
            workbook.Save("SeriesOverlapDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


