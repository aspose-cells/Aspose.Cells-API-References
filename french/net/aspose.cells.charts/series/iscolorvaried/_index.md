---
title: "Series.IsColorVaried"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Indique si la couleur des points varie. Le graphique doit contenir une seule série ou être un graphique circulaire"
type: docs
url: /fr/net/aspose.cells.charts/series/iscolorvaried/
---
## Series.IsColorVaried property

Indique si la couleur des points varie. Le graphique doit contenir une seule série ou être un graphique circulaire.

```csharp
public bool IsColorVaried { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsColorVariedDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir la propriété IsColorVaried pour la première série
            chart.NSeries[0].IsColorVaried = true;

            // Enregistrez le classeur
            workbook.Save("output.xlsx");

            // Vérifier la propriété
            Console.WriteLine("IsColorVaried: " + chart.NSeries[0].IsColorVaried);
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


