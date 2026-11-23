---
title: "Axis.CategoryType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Axis. Représente le type de l'axe des catégories"
type: docs
url: /fr/net/aspose.cells.charts/axis/categorytype/
---
## Axis.CategoryType property

Représente le type de l'axe de catégorie.

```csharp
public CategoryType CategoryType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyCategoryTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 2, 25, 11);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("=Sheet1!$A$1:$B$10", true);

            // Démontrer la propriété CategoryType
            chart.CategoryAxis.CategoryType = Aspose.Cells.Charts.CategoryType.AutomaticScale;
            Console.WriteLine("CategoryType set to AutomaticScale");

            // Enregistrez le classeur
            workbook.Save("AxisPropertyCategoryTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [CategoryType](../../categorytype/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


