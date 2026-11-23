---
title: "Series.ValuesFormatCode"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Représente le code de format de la Values NumberList"
type: docs
url: /fr/net/aspose.cells.charts/series/valuesformatcode/
---
## Series.ValuesFormatCode property

Représente le code de format de la liste de nombres des valeurs.

```csharp
public string ValuesFormatCode { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyValuesFormatCodeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(0.25);
            worksheet.Cells["B3"].PutValue(0.5);
            worksheet.Cells["B4"].PutValue(0.75);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Définir le code de format des valeurs pour la première série
            chart.NSeries[0].ValuesFormatCode = "0.00%";

            // Enregistrez le classeur
            workbook.Save("SeriesPropertyValuesFormatCodeDemo_out.xlsx");
        }
    }
}
```

### Voir aussi

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


