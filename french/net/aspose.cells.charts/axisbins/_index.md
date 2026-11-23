---
title: "Classe AxisBins"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.AxisBins. Représente les intervalles d'axe"
type: docs
url: /fr/net/aspose.cells.charts/axisbins/
---
## AxisBins class

Représente les intervalles d'axe

```csharp
public class AxisBins
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Count](../../aspose.cells.charts/axisbins/count/) { get; set; } | Obtient ou définit le nombre d'intervalles d'axe |
| [IsAutomatic](../../aspose.cells.charts/axisbins/isautomatic/) { get; set; } | Indique si les intervalles d'axe sont automatiques. |
| [IsByCategory](../../aspose.cells.charts/axisbins/isbycategory/) { get; set; } | Indique si le regroupement des données par catégorie est activé. |
| [Overflow](../../aspose.cells.charts/axisbins/overflow/) { get; set; } | Obtient ou définit le dépassement des intervalles d'axe |
| [Underflow](../../aspose.cells.charts/axisbins/underflow/) { get; set; } | Obtient ou définit le sous-dépassement des intervalles d'axe |
| [Width](../../aspose.cells.charts/axisbins/width/) { get; set; } | Obtient ou définit la largeur de l'intervalle d'axe. |

## Méthodes

| Nom | Description |
| --- | --- |
| [ResetOverflow](../../aspose.cells.charts/axisbins/resetoverflow/)() | (**Obsolete.**) Réinitialiser le dépassement |
| [ResetUnderflow](../../aspose.cells.charts/axisbins/resetunderflow/)() | (**Obsolete.**) Réinitialiser le sous-dépassement |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class AxisBinsDemo
    {
        public static void AxisBinsExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            // Ajouter une nouvelle feuille de calcul
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);
            worksheet.Cells["A5"].PutValue(50);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = worksheet.Charts.Add(ChartType.Histogram, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Ajouter une série de données au graphique
            chart.NSeries.Add("A1:A5", true);

            // Accéder à l'axe des valeurs
            Axis valueAxis = chart.ValueAxis;

            // Accéder aux intervalles de l'axe des valeurs
            AxisBins bins = valueAxis.Bins;

            // Définir les propriétés des intervalles
            bins.IsByCategory = false;
            bins.IsAutomatic = true;
            bins.Width = 10.0;
            bins.Count = 5;
            bins.Overflow = 60.0;
            bins.Underflow = 0.0;

            // Réinitialiser le dépassement et le sous-dépassement
            //bins.ResetOverflow();
            //bins.ResetUnderflow();

            // Enregistrez le classeur
            workbook.Save("AxisBinsExample.xlsx");
            workbook.Save("AxisBinsExample.pdf");
        }
    }
}
```

### Voir aussi

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


