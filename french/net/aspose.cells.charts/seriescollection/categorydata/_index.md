---
title: "SeriesCollection.CategoryData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SeriesCollection. Obtient ou définit la plage des valeurs de l'axe des catégories. Cela peut être une plage de cellules comme d1e10 ou une séquence de valeurs comme 26810"
type: docs
url: /fr/net/aspose.cells.charts/seriescollection/categorydata/
---
## SeriesCollection.CategoryData property

Obtient ou définit la plage des valeurs de l'axe des catégories. Elle peut être une plage de cellules (par exemple "d1:e10") ou une séquence de valeurs (par exemple "{2,6,8,10}").

```csharp
public string CategoryData { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertyCategoryDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            
            // Accéder à la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                worksheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                worksheet.Cells["B" + i].PutValue(i * 10);
            }
            
            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données du graphique
            chart.NSeries.Add("=Sheet1!$B$2:$B$10", true);
            chart.NSeries.CategoryData = "=Sheet1!$A$2:$A$10";
            
            // Enregistrez le classeur
            workbook.Save("CategoryDataDemo.xlsx");
            
            // Vérifiez la propriété CategoryData
            Console.WriteLine("Chart CategoryData: " + chart.NSeries.CategoryData);
        }
    }
}
```

### Voir aussi

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


