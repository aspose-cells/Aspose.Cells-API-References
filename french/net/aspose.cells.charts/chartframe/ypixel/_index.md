---
title: "ChartFrame.YPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient ou définit la coordonnée y du coin supérieur gauche en unités de pixels"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/ypixel/
---
## ChartFrame.YPixel property

Obtient ou définit la coordonnée y du coin supérieur gauche en unités de pixels.

```csharp
public virtual int YPixel { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyYPixelDemo
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

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Accéder au titre du graphique (qui hérite de ChartFrame)
            chart.Title.Text = "Sample Chart";
            ChartFrame chartFrame = chart.Title;

            // Afficher la valeur actuelle de YPixel
            Console.WriteLine("Current YPixel value: " + chartFrame.YPixel);

            // Modifier la position YPixel du titre du graphique
            chartFrame.YPixel = 50;
            Console.WriteLine("New YPixel value: " + chartFrame.YPixel);

            // Enregistrez le classeur
            workbook.Save("ChartFrameYPixelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


