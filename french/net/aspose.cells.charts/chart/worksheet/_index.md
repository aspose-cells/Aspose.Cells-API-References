---
title: "Chart.Worksheet"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Obtient la feuille de calcul qui contient ce graphique"
type: docs
url: /fr/net/aspose.cells.charts/chart/worksheet/
---
## Chart.Worksheet property

Obtient la feuille de calcul qui contient ce graphique.

```csharp
public Worksheet Worksheet { get; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyWorksheetDemo
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
            
            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Démontrer l'utilisation de la propriété Worksheet
            Console.WriteLine("Chart's worksheet index: " + chart.Worksheet.Index);
            Console.WriteLine("Chart's worksheet name: " + chart.Worksheet.Name);
            
            // Enregistrez le classeur
            workbook.Save("ChartPropertyWorksheetDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


