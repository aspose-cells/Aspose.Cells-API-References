---
title: "ErrorBar.MinusValue"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété ErrorBar. Représente la quantité d'erreur négative lorsque le type de barre d'erreur est Personnalisé"
type: docs
url: /fr/net/aspose.cells.charts/errorbar/minusvalue/
---
## ErrorBar.MinusValue property

Représente la quantité d'erreur négative lorsque le type de barre d'erreur est Personnalisé.

```csharp
public string MinusValue { get; set; }
```

### Exemples

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyMinusValueDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(5);
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(15);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter une série
            chart.NSeries.Add("B2:B3", true);

            // Configurer les barres d'erreur
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.DisplayType = ErrorBarDisplayType.Both;
            errorBar.Type = ErrorBarType.Custom;
            errorBar.PlusValue = "=A2";
            errorBar.MinusValue = "=A3";

            // Enregistrez le classeur
            workbook.Save("ErrorBarMinusValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


