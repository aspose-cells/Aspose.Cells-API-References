---
title: "Legend.LegendEntriesLabels"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Legend. Obtient les libellés des entrées de légende après l'appel de la méthode Chart.Calculate"
type: docs
url: /fr/net/aspose.cells.charts/legend/legendentrieslabels/
---
## Legend.LegendEntriesLabels property

Obtient les libellés des entrées de légende après l'appel de la méthode Chart.Calculate().

```csharp
[Obsolete("Use Legend.GetLegendLabels method, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ArrayList LegendEntriesLabels { get; }
```

### Remarques

NOTE: Ce membre est maintenant obsolète. À la place, veuillez utiliser la méthode Legend.GetLegendLabels. Cette propriété sera supprimée 12 mois plus tard à compter de novembre 2023. Aspose s'excuse pour tout inconvénient que vous avez pu rencontrer.

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPropertyLegendEntriesLabelsDemo
    {
        public static void Run()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple pour le graphique
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajoutez un graphique
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Définir la source de données du graphique
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calculer le graphique pour garantir que les entrées de légende sont générées
            chart.Calculate();

            // Obtenir la légende
            Legend legend = chart.Legend;

            // Afficher les libellés des entrées de légende (en utilisant la propriété)
            Console.WriteLine("Legend Entries Labels:");
            foreach (string label in legend.LegendEntriesLabels)
            {
                Console.WriteLine(label);
            }

            // Enregistrez le classeur
            workbook.Save("LegendEntriesLabelsDemo.xlsx");
        }
    }
}
```

### Voir aussi

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


