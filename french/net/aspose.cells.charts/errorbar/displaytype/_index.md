---
title: "ErrorBar.DisplayType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ErrorBar. Représente le type d'affichage de la barre d'erreur"
type: docs
url: /fr/net/aspose.cells.charts/errorbar/displaytype/
---
## ErrorBar.DisplayType property

Représente le type d'affichage de la barre d'erreur.

```csharp
public ErrorBarDisplayType DisplayType { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyDisplayTypeDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter une série
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Définir le type d'affichage de la barre d'erreur
            chart.NSeries[0].YErrorBar.DisplayType = ErrorBarDisplayType.Plus;

            // Enregistrez le classeur
            workbook.Save("ErrorBarDisplayTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* enum [ErrorBarDisplayType](../../errorbardisplaytype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


