---
title: "Enum PrintSizeType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Enum Aspose.Cells.PrintSizeType. Représente la taille du graphique imprimé"
type: docs
url: /fr/net/aspose.cells/printsizetype/
---
## PrintSizeType enumeration

Représente la taille du graphique imprimé.

```csharp
public enum PrintSizeType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Full | `0` | Utiliser la pleine page. |
| Fit | `1` | Échelle pour ajuster à la page. |
| Custom | `2` | Personnalisé. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PrintSizeTypeDemo
    {
        public static void PrintSizeTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Obtenir la première feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données pour le graphique
            chart.SetChartDataRange("A1:B4", true);

            // Définir le titre du graphique
            chart.Title.Text = "Sample Chart";

            // Définir la taille d'impression du graphique
            chart.PrintSize = PrintSizeType.Fit;

            // Enregistrez le classeur
            workbook.Save("PrintSizeTypeExample.xlsx");

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


