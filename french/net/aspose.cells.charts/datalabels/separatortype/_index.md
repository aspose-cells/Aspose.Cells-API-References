---
title: "DataLabels.SeparatorType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété DataLabels. Obtient ou définit le type de séparateur utilisé pour les étiquettes de données sur un graphique"
type: docs
url: /fr/net/aspose.cells.charts/datalabels/separatortype/
---
## DataLabels.SeparatorType property

Obtient ou définit le type de séparateur utilisé pour les étiquettes de données sur un graphique.

```csharp
public DataLabelsSeparatorType SeparatorType { get; set; }
```

### Remarques

Pour définir un séparateur personnalisé, veuillez définir la propriété `SeparatorType` sur Custom puis spécifier la valeur attendue pour [`SeparatorValue`](../separatorvalue/).

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertySeparatorTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Activer les étiquettes de données
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.ShowCategoryName = true;
            
            // Définir le type de séparateur
            chart.NSeries[0].DataLabels.SeparatorType = DataLabelsSeparatorType.Space;

            // Enregistrez le classeur
            workbook.Save("DataLabelsSeparatorTypeDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [DataLabelsSeparatorType](../../datalabelsseparatortype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


