---
title: "Enum MsoLineStyle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Drawing.MsoLineStyle. Représente le style des lignes de dessin"
type: docs
url: /fr/net/aspose.cells.drawing/msolinestyle/
---
## MsoLineStyle enumeration

Représente le style des lignes de dessin.

```csharp
public enum MsoLineStyle
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Single | `0` | Ligne simple (de largeur lineWidth) |
| ThickBetweenThin | `1` | Trois lignes, fine, épaisse, fine |
| ThinThick | `2` | Lignes doubles, une fine, une épaisse |
| ThickThin | `3` | Lignes doubles, une épaisse, une fine |
| ThinThin | `4` | Lignes doubles de largeur égale |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoLineStyleDemo
    {
        public static void MsoLineStyleExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();

            // Ajouter une nouvelle feuille de calcul au classeur
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.SetChartDataRange("A1:B4", true);

            // Accéder à l'axe de catégorie principal
            Axis categoryAxis = chart.CategoryAxis;

            // Définir le style de ligne pour l'axe de catégorie principal
            Line axisLine = categoryAxis.AxisLine;
            axisLine.CompoundType = MsoLineStyle.ThickBetweenThin;
            axisLine.Color = Color.Blue;
            axisLine.WeightPt = 2.0;

            // Afficher le style de ligne
            Console.WriteLine("Axis Line Style: " + axisLine.CompoundType);
            Console.WriteLine("Axis Line Color: " + axisLine.Color);
            Console.WriteLine("Axis Line Weight: " + axisLine.WeightPt);

            // Enregistrez le classeur
            workbook.Save("MsoLineStyleExample.xlsx");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


