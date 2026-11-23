---
title: "Title.X"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Title. Obtient ou définit la coordonnée X du coin supérieur gauche en unités de 1/4000 de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/title/x/
---
## Title.X property

Obtient ou définit la coordonnée X du coin supérieur gauche en unités de 1/4000 de la zone du graphique.

```csharp
[Obsolete("Use Title.XRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int X { get; set; }
```

### Remarques

NOTE : Ce membre est désormais obsolète. Veuillez utiliser la propriété Title.XRatioToChart à la place. X = XRatioToChart * 4000 ; Cette propriété sera supprimée 12 mois plus tard, à compter de février 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TitlePropertyXDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);

            // Ajoutez un graphique et définissez les données
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            // Définissez les propriétés du titre du graphique avec la position X
            chart.Title.Text = "Sample Chart";
            chart.Title.X = 200; // Demonstrating X property usage
            chart.Title.Y = 50;

            // Enregistrez le classeur
            workbook.Save("TitlePropertyXDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


