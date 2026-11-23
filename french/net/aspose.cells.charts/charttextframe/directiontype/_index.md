---
title: "ChartTextFrame.DirectionType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ChartTextFrame. Obtient et définit la direction du texte"
type: docs
url: /fr/net/aspose.cells.charts/charttextframe/directiontype/
---
## ChartTextFrame.DirectionType property

Obtient et définit la direction du texte.

```csharp
public virtual ChartTextDirectionType DirectionType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyDirectionTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            // L'ajout d'une feuille de calcul renvoie son indice, puis nous récupérons la feuille de calcul par indice
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);
            chart.NSeries.CategoryData = "C1:C3";

            // Accéder et configurer le titre
            ChartTextFrame title = chart.Title;
            title.Text = "Sample Chart";
            
            // Démontrer la propriété DirectionType
            title.DirectionType = ChartTextDirectionType.Vertical;
            
            // Enregistrez le classeur
            workbook.Save("ChartTextDirectionDemo.xlsx");
        }
    }
}
```

### Voir aussi

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


