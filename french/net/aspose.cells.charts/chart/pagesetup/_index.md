---
title: "Chart.PageSetup"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Représente la description de la configuration de page dans ce graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/pagesetup/
---
## Chart.PageSetup property

Représente la description de la mise en page dans ce graphique.

```csharp
public PageSetup PageSetup { get; }
```

### Exemples

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyPageSetupDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Ajouter une feuille de calcul et insérer des données pour le graphique
            Worksheet dataSheet = workbook.Worksheets[workbook.Worksheets.Add()];
            dataSheet.Name = "DataSheet";
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["A4"].PutValue("C");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["B4"].PutValue(30);

            // Ajouter une feuille de graphique
            int chartSheetIndex = workbook.Worksheets.Add(SheetType.Chart);
            Worksheet chartSheet = workbook.Worksheets[chartSheetIndex];
            chartSheet.Name = "ChartSheet";

            // Ajouter un graphique à la feuille de graphique
            int chartIndex = chartSheet.Charts.Add(ChartType.Column, 0, 0, 800, 600);
            Chart chart = chartSheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Accéder à la configuration de page du graphique
            PageSetup pageSetup = chart.PageSetup;

            // Définir les propriétés de mise en page
            pageSetup.Orientation = PageOrientationType.Landscape;
            pageSetup.PaperSize = PaperSizeType.PaperA4;
            pageSetup.Zoom = 90;
            pageSetup.LeftMargin = 2.0;
            pageSetup.RightMargin = 2.0;
            pageSetup.TopMargin = 2.0;
            pageSetup.BottomMargin = 2.0;

            // Définir l'en-tête avec du texte et une image
            byte[] imageData = File.ReadAllBytes("logo.png");
            pageSetup.SetHeaderPicture(0, imageData);
            pageSetup.SetHeader(0, "&G");
            pageSetup.SetHeader(1, "Sales Report");
            pageSetup.SetHeader(2, "&D");

            // Définir le pied de page
            pageSetup.SetFooter(0, "Page &P of &N");

            // Enregistrez le classeur
            workbook.Save("ChartPageSetupDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [PageSetup](../../../aspose.cells/pagesetup/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


