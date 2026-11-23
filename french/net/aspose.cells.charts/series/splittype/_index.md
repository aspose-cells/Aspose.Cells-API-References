---
title: "Series.SplitType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Renvoie ou définit une valeur qui détermine quels points de données se trouvent dans le deuxième secteur ou barre d'un graphique en secteur de secteur ou barre de secteur."
type: docs
url: /fr/net/aspose.cells.charts/series/splittype/
---
## Series.SplitType property

Renvoie ou définit une valeur qui détermine quels points de données se trouvent dans le deuxième secteur ou la deuxième barre d'un graphique en secteurs de secteurs ou en barres de secteurs.

```csharp
public ChartSplitType SplitType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitTypeDemo
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
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique en secteurs
            int chartIndex = sheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir le type de division pour la première série
            chart.NSeries[0].SplitType = ChartSplitType.Position;

            // Enregistrez le classeur
            workbook.Save("SeriesPropertySplitTypeDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ChartSplitType](../../chartsplittype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


