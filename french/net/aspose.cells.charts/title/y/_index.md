---
title: "Title.Y"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Title. Obtient ou définit la coordonnée y du coin supérieur gauche en unités de 1/4000 de la zone du graphique"
type: docs
url: /fr/net/aspose.cells.charts/title/y/
---
## Title.Y property

Obtient ou définit la coordonnée y du coin supérieur gauche en unités de 1/4000 de la zone du graphique.

```csharp
[Obsolete("Use Title.YRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public override int Y { get; set; }
```

### Remarques

NOTE : Ce membre est désormais obsolète. Veuillez utiliser la propriété Title.YRatioToChart à la place. Y = YRatioToChart * 4000 ; Cette propriété sera supprimée 12 mois plus tard, à compter de février 2025. Aspose s’excuse pour tout désagrément que vous auriez pu rencontrer.

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class TitlePropertyYDemo
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir le titre du graphique
            chart.Title.Text = "Sample Chart";
            chart.Title.Y = 1000; // Demonstrating Y property - position in 1/4000 units
            
            // Calculez le graphique pour garantir que la mise en page est mise à jour
            chart.Calculate();

            // Ajoutez une forme alignée avec la position Y du titre
            Shape shape = chart.Shapes.AddShapeInChart(MsoDrawingType.Rectangle, PlacementType.Move,
                2000, 
                chart.Title.Y, // Using the title's Y property
                3000, 
                chart.Title.Y + 500);
            shape.Fill.SolidFill.Color = Color.Blue;

            // Enregistrez le classeur
            workbook.Save("TitlePropertyYDemo_Output.xlsx");
        }
    }
}
```

### Voir aussi

* class [Title](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


