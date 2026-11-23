---
title: "ChartTextFrame.IsResizeShapeToFitText"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartTextFrame. Obtient ou définit si une forme doit être automatiquement ajustée pour contenir entièrement le texte qui y est décrit. L'ajustement automatique consiste à mettre à l'échelle le texte à l'intérieur d'une forme afin de contenir tout le texte."
type: docs
url: /fr/net/aspose.cells.charts/charttextframe/isresizeshapetofittext/
---
## ChartTextFrame.IsResizeShapeToFitText property

Obtient ou définit si une forme doit être ajustée automatiquement pour contenir entièrement le texte qui y est décrit. L'ajustement automatique consiste à mettre à l'échelle le texte à l'intérieur d'une forme afin de contenir tout le texte.

```csharp
public bool IsResizeShapeToFitText { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsResizeShapeToFitTextDemo
    {
        public static void Run()
        {
            // Créer un classeur
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Ajouter un graphique en colonnes
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir les données de la série
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Accéder aux étiquettes de données
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.Center;

            // Démontrer la propriété IsResizeShapeToFitText
            foreach (ChartPoint point in chart.NSeries[0].Points)
            {
                // Désactiver le redimensionnement automatique de la forme pour ajuster le texte
                point.DataLabels.IsResizeShapeToFitText = false;
                
                // Définir une largeur personnalisée inférieure à celle requise normalement par le texte
                point.DataLabels.Width = 50;
            }

            // Enregistrez le classeur
            workbook.Save("ChartTextFramePropertyIsResizeShapeToFitTextDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


