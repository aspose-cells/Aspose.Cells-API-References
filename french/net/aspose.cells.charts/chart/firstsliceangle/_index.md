---
title: "Chart.FirstSliceAngle"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Chart. Obtient ou définit l'angle de la première tranche de diagramme circulaire ou de diagramme en anneau en degrés, dans le sens des aiguilles d'une montre à partir du vertical. S'applique uniquement aux graphiques circulaires 3D et aux graphiques en anneau de 0 à 360"
type: docs
url: /fr/net/aspose.cells.charts/chart/firstsliceangle/
---
## Chart.FirstSliceAngle property

Obtient ou définit l'angle de la première tranche de diagramme circulaire ou de diagramme en anneau, en degrés (dans le sens des aiguilles d'une montre depuis la verticale). S'applique uniquement aux diagrammes circulaires, 3D circulaires et en anneau, de 0 à 360.

```csharp
public int FirstSliceAngle { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFirstSliceAngleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Ajouter un graphique circulaire
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Pie, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir la plage de données
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Définir l'angle de la première tranche à 45 degrés
            chart.FirstSliceAngle = 45;
            
            // Enregistrez le classeur
            workbook.Save("PieChartWithFirstSliceAngle.xlsx");
        }
    }
}
```

### Voir aussi

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


