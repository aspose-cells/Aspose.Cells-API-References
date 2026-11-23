---
title: "Classe SparklineGroupCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.Charts.SparklineGroupCollection. Encapsule une collection d'objets SparklineGroup"
type: docs
url: /fr/net/aspose.cells.charts/sparklinegroupcollection/
---
## SparklineGroupCollection class

Encapsule une collection d'objets [`SparklineGroup`](../sparklinegroup/).

```csharp
public class SparklineGroupCollection : CollectionBase<SparklineGroup>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.charts/sparklinegroupcollection/item/) { get; } | Obtient l'élément [`SparklineGroup`](../sparklinegroup/) à l'index spécifié. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [Add](../../aspose.cells.charts/sparklinegroupcollection/add/#add)(SparklineType) | Ajoute un [`SparklineGroup`](../sparklinegroup/) avec un [`Sparkline`](../sparkline/) à la collection. |
| [Add](../../aspose.cells.charts/sparklinegroupcollection/add/#add_1)(SparklineType, string, bool, CellArea) | Ajoute un [`SparklineGroup`](../sparklinegroup/) avec plusieurs [`Sparkline`](../sparkline/) à la collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SparklineGroup) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SparklineGroup, IComparer&lt;SparklineGroup&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, SparklineGroup, IComparer&lt;SparklineGroup&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [ClearSparklineGroups](../../aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups/)(CellArea) | Efface les groupes de sparkline qui se chevauchent avec une zone de cellules. |
| [ClearSparklines](../../aspose.cells.charts/sparklinegroupcollection/clearsparklines/)(CellArea) | Efface les sparklines qui se trouvent à l'intérieur d'une zone de cellules. |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(SparklineGroup) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SparklineGroup[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SparklineGroup[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, SparklineGroup[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;SparklineGroup&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;SparklineGroup&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;SparklineGroup&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SparklineGroup) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SparklineGroup, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SparklineGroup, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SparklineGroup) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SparklineGroup, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SparklineGroup, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineGroupCollectionDemo
    {
        public static void SparklineGroupCollectionExample()
        {
            // Créer un nouveau classeur
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Ajouter des données à la feuille de calcul
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Définit la CellArea pour le sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Ajoute un groupe de sparklines à la feuille de calcul
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Ajoute des sparklines au groupe
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 5);

            // Personnalisez le groupe de sparkline
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;
            group.LineWeight = 1.0;

            // Enregistrez le classeur
            workbook.Save("SparklineGroupCollectionExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [SparklineGroup](../sparklinegroup/)
* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


