---
title: "Chart.Floor"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Retourne un objet Floor qui représente les parois d’un graphique 3D"
type: docs
url: /fr/net/aspose.cells.charts/chart/floor/
---
## Chart.Floor property

Retourne un objet `Floor` qui représente les parois d’un graphique 3 D.

```csharp
public Floor Floor { get; }
```

### Remarques

Cette propriété ne s'applique pas aux graphiques circulaires 3-D.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartPropertyFloorDemo
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

            // Ajouter un graphique à colonnes 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder et modifier les propriétés du plancher
            Floor floor = chart.Floor;
            floor.FillFormat.SetTwoColorGradient(System.Drawing.Color.LightBlue, System.Drawing.Color.DarkBlue, GradientStyleType.Horizontal, 2);
            floor.Border.Color = System.Drawing.Color.Black;

            // Enregistrez le classeur
            workbook.Save("ChartFloorDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Floor](../../floor/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


