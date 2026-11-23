---
title: "SeriesCollection.SecondCategoryData"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété SeriesCollection. Obtient ou définit la plage des valeurs du deuxième axe des catégories. Cela peut être une plage de cellules comme d1e10 ou une séquence de valeurs comme 26810. N'affecte que lorsque certaines séries sont tracées sur le deuxième axe"
type: docs
url: /fr/net/aspose.cells.charts/seriescollection/secondcategorydata/
---
## SeriesCollection.SecondCategoryData property

Obtient ou définit la plage des valeurs du deuxième axe des catégories. Elle peut être une plage de cellules (par exemple "d1:e10"), ou une séquence de valeurs (par exemple "{2,6,8,10}"). N'affecte que lorsque certaines séries sont tracées sur le deuxième axe.

```csharp
public string SecondCategoryData { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesCollectionPropertySecondCategoryDataDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Primary Categories");
            worksheet.Cells["A2"].PutValue("Cat1");
            worksheet.Cells["A3"].PutValue("Cat2");
            worksheet.Cells["A4"].PutValue("Cat3");
            
            worksheet.Cells["B1"].PutValue("Secondary Categories");
            worksheet.Cells["B2"].PutValue("SubCat1");
            worksheet.Cells["B3"].PutValue("SubCat2");
            worksheet.Cells["B4"].PutValue("SubCat3");
            
            worksheet.Cells["C1"].PutValue("Values");
            worksheet.Cells["C2"].PutValue(10);
            worksheet.Cells["C3"].PutValue(20);
            worksheet.Cells["C4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir les données de la série
            chart.NSeries.Add("C2:C4", true);
            
            // Définir les données de la catégorie principale
            chart.NSeries.CategoryData = "A2:A4";
            
            // Définir les données de la catégorie secondaire
            chart.NSeries.SecondCategoryData = "B2:B4";

            // Enregistrez le classeur
            workbook.Save("SecondCategoryDataDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [SeriesCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


