---
title: "ChartFrame.WidthPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient ou définit la largeur du cadre en unités de Pixel"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/widthpixel/
---
## ChartFrame.WidthPixel property

Obtient ou définit la largeur du cadre en unités de Pixel.

```csharp
public virtual int WidthPixel { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyWidthPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accéder au titre du graphique (qui hérite de ChartFrame)
            chart.Title.Text = "Sample Chart";
            
            // Afficher la valeur actuelle de WidthPixel du titre du graphique
            Console.WriteLine("Current Title WidthPixel: " + chart.Title.WidthPixel);
            
            // Définir une nouvelle largeur pour le titre du graphique en pixels
            chart.Title.WidthPixel = 300;
            
            // Afficher la nouvelle valeur de WidthPixel
            Console.WriteLine("New Title WidthPixel: " + chart.Title.WidthPixel);
            
            // Enregistrez le classeur
            workbook.Save("ChartFrameWidthPixelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


