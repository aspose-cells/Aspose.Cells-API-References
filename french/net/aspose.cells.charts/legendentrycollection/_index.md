---
title: "Classe LegendEntryCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.LegendEntryCollection. Représente une collection de tous les objets LegendEntry dans la légende du graphique spécifiée"
type: docs
url: /fr/net/aspose.cells.charts/legendentrycollection/
---
## LegendEntryCollection class

Représente une collection de tous les objets [`LegendEntry`](../legendentry/) dans la légende du graphique spécifiée.

```csharp
public class LegendEntryCollection : CollectionBase<LegendEntry>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/legendentrycollection/item/) { get; } | Obtient l'élément [`LegendEntry`](../legendentry/) à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(LegendEntry) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(LegendEntry, IComparer&lt;LegendEntry&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, LegendEntry, IComparer&lt;LegendEntry&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(LegendEntry) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(LegendEntry[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(LegendEntry[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, LegendEntry[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;LegendEntry&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;LegendEntry&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;LegendEntry&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;LegendEntry&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;LegendEntry&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;LegendEntry&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;LegendEntry&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;LegendEntry&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;LegendEntry&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;LegendEntry&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(LegendEntry) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(LegendEntry, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(LegendEntry, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(LegendEntry) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(LegendEntry, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(LegendEntry, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryCollectionDemo
    {
        public static void LegendEntryCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajoutez des données pour le graphique
            sheet.Cells[0, 1].PutValue("Income");
            sheet.Cells[1, 0].PutValue("Company A");
            sheet.Cells[2, 0].PutValue("Company B");
            sheet.Cells[3, 0].PutValue("Company C");
            sheet.Cells[1, 1].PutValue(10000);
            sheet.Cells[2, 1].PutValue(20000);
            sheet.Cells[3, 1].PutValue(30000);

            // Ajouter un graphique à la feuille de calcul
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Accédez à la légende du graphique
            Legend legend = chart.Legend;

            // Accédez à la collection des entrées de légende
            LegendEntryCollection legendEntries = legend.LegendEntries;

            // Modifiez les propriétés de la première entrée de légende
            if (legendEntries.Count > 0)
            {
                LegendEntry firstEntry = legendEntries[0];
                firstEntry.IsDeleted = false;
                firstEntry.AutoScaleFont = true;
                firstEntry.Background = BackgroundMode.Transparent;
            }

            // Enregistrez le classeur
            workbook.Save("LegendEntryCollectionExample.xlsx");
            workbook.Save("LegendEntryCollectionExample.pdf");
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [LegendEntry](../legendentry/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


