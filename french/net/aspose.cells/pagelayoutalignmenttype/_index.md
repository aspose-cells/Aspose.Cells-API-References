---
title: "Enum PageLayoutAlignmentType"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.PageLayoutAlignmentType enum. Énumère les types d'alignement de mise en page"
type: docs
url: /fr/net/aspose.cells/pagelayoutalignmenttype/
---
## PageLayoutAlignmentType enumeration

Énumère les types d'alignement de la mise en page.

```csharp
public enum PageLayoutAlignmentType
```

### Valeurs

| Nom | Valeur | Description |
| --- | --- | --- |
| Bottom | `0` | Représente l'alignement de mise en page inférieur. |
| Center | `1` | Représente l'alignement de mise en page central. |
| Left | `2` | Représente l'alignement de mise en page à gauche. |
| Right | `3` | Représente l'alignement de mise en page à droite. |
| Top | `4` | Représente l'alignement de mise en page supérieur. |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PageLayoutAlignmentTypeDemo
    {
        public static void PageLayoutAlignmentTypeExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(456);
            worksheet.Cells["A4"].PutValue(789);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Définir la plage de données pour le graphique
            chart.SetChartDataRange("A1:A4", true);

            // Définir le titre du graphique
            chart.Title.Text = "Sample Chart";

            // Enregistrer le classeur dans un fichier
            workbook.Save("PageLayoutAlignmentTypeExample.xlsx");

            // Exporter le graphique en PDF avec un alignement de mise en page spécifique
            chart.ToPdf("ChartExample.pdf", 8.5f, 11f, PageLayoutAlignmentType.Center, PageLayoutAlignmentType.Center);

            return;
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


