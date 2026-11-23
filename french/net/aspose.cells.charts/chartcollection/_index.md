---
title: "Classe ChartCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Aspose.Cells.Charts.ChartCollection class. Encapsule une collection d'objets Chart"
type: docs
url: /fr/net/aspose.cells.charts/chartcollection/
---
## ChartCollection class

Encapsule une collection d'objets [`Chart`](../chart/).

```csharp
public class ChartCollection : CollectionBase<Chart>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/chartcollection/item/) { get; } | Obtient l'élément [`Chart`](../chart/) à l'index spécifié. (2 indexeurs) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.charts/chartcollection/add/#add)(ChartType, int, int, int, int) | Ajoute un graphique à la collection. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_2)(ChartType, string, int, int, int, int) | (**Obsolète.**) Ajoute un graphique à la collection. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_3)(byte[], string, bool, int, int, int, int) | Ajoute un graphique avec un modèle prédéfini. |
| [Add](../../aspose.cells.charts/chartcollection/add/#add_1)(ChartType, string, bool, int, int, int, int) | Ajoute un graphique à la collection. |
| [AddFloatingChart](../../aspose.cells.charts/chartcollection/addfloatingchart/)(ChartType, int, int, int, int) | Ajoute un graphique à la collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Chart) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Chart, IComparer&lt;Chart&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Chart, IComparer&lt;Chart&gt;) |  |
| [Clear](../../aspose.cells.charts/chartcollection/clear/#clear)() | Efface tous les graphiques. (2 méthodes) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Chart) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Chart[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Chart[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Chart[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Chart&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Chart&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Chart&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Chart&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Chart&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Chart&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Chart, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Chart, int, int) |  |
| [RemoveAt](../../aspose.cells.charts/chartcollection/removeat/#removeat)(int) | Supprime un graphique à l'index spécifié. (2 méthodes) |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartCollectionDemo
    {
        public static void ChartCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ajouter des données d'exemple à la feuille de calcul
            worksheet.Cells[0, 0].PutValue("Category");
            worksheet.Cells[0, 1].PutValue("Value");
            worksheet.Cells[1, 0].PutValue("A");
            worksheet.Cells[1, 1].PutValue(10);
            worksheet.Cells[2, 0].PutValue("B");
            worksheet.Cells[2, 1].PutValue(20);
            worksheet.Cells[3, 0].PutValue("C");
            worksheet.Cells[3, 1].PutValue(30);

            // Accéder à la collection de graphiques de la feuille de calcul
            ChartCollection charts = worksheet.Charts;

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = charts[chartIndex];

            // Définir la plage de données pour le graphique
            chart.SetChartDataRange("A1:B4", true);

            // Personnaliser le graphique
            chart.Title.Text = "Sample Chart";
            chart.ShowLegend = true;

            // Enregistrez le classeur
            workbook.Save("ChartCollectionExample.xlsx");
            workbook.Save("ChartCollectionExample.pdf");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [Chart](../chart/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


