---
title: "ChartFrame.HeightPixel"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartFrame. Obtient ou définit la hauteur du cadre en unités de pixels"
type: docs
url: /fr/net/aspose.cells.charts/chartframe/heightpixel/
---
## ChartFrame.HeightPixel property

Obtient ou définit la hauteur du cadre en unités de pixels.

```csharp
public virtual int HeightPixel { get; set; }
```

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartFramePropertyHeightPixelDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Accéder au titre du graphique (qui est un ChartFrame)
            ChartFrame chartTitle = chart.Title;
            
            // Afficher la hauteur actuelle en pixels
            Console.WriteLine("Current title height: " + chartTitle.HeightPixel + " pixels");
            
            // Définir une nouvelle hauteur pour le titre
            chartTitle.HeightPixel = 40;
            Console.WriteLine("New title height: " + chartTitle.HeightPixel + " pixels");
            
            // Accéder à la légende (un autre ChartFrame)
            ChartFrame legend = chart.Legend;
            
            // Afficher et modifier la hauteur de la légende
            Console.WriteLine("Current legend height: " + legend.HeightPixel + " pixels");
            legend.HeightPixel = 60;
            Console.WriteLine("New legend height: " + legend.HeightPixel + " pixels");
            
            // Enregistrez le classeur
            workbook.Save("ChartFrameHeightPixelDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


