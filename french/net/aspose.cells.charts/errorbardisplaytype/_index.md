---
title: "Enum ErrorBarDisplayType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.Charts.ErrorBarDisplayType. Représente le type d'affichage de la barre d'erreur"
type: docs
url: /fr/net/aspose.cells.charts/errorbardisplaytype/
---
## ErrorBarDisplayType enumeration

Représente le type d'affichage de la barre d'erreur.

```csharp
public enum ErrorBarDisplayType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Both | `0` | Les deux |
| Minus | `1` | Moins |
| None | `2` | Aucun |
| Plus | `3` | Plus |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarDisplayTypeDemo
    {
        public static void ErrorBarDisplayTypeExample()
        {
            // Créer un nouveau classeur et accéder à la première feuille de calcul
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            worksheet.Cells["A1"].PutValue(2);
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(6);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(7);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Ajoutez un graphique en colonnes à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Configurez les barres d'erreur pour chaque série du graphique
            foreach (Series series in chart.NSeries)
            {
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Enregistrez le classeur
            workbook.Save("ErrorBarDisplayTypeExample.xlsx");
            workbook.Save("ErrorBarDisplayTypeExample.pdf");
            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


