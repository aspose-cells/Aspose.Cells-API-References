---
title: "Chart.SizeWithWindow"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Chart property. Vrai si Microsoft Excel redimensionne le graphique pour correspondre à la taille de la fenêtre de la feuille de graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/sizewithwindow/
---
## Chart.SizeWithWindow property

Vrai si Microsoft Excel redimensionne le graphique pour correspondre à la taille de la fenêtre de la feuille de graphique.

```csharp
public bool SizeWithWindow { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySizeWithWindowDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
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
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Démontrer la propriété SizeWithWindow
            Console.WriteLine("Default SizeWithWindow: " + chart.SizeWithWindow);
            
            // Activer SizeWithWindow
            chart.SizeWithWindow = true;
            Console.WriteLine("After setting SizeWithWindow to true: " + chart.SizeWithWindow);
            
            // Enregistrez le classeur
            workbook.Save("ChartSizeWithWindowDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


