---
title: "Classe ReferredAreaCollection"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Classe Aspose.Cells.ReferredAreaCollection. Représente toutes les cellules et zones référencées"
type: docs
url: /fr/net/aspose.cells/referredareacollection/
---
## ReferredAreaCollection class

Représente toutes les cellules et zones référencées.

```csharp
public class ReferredAreaCollection : CollectionBase<ReferredArea>
```

## Propriétés

| Nom | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/referredareacollection/item/) { get; } |  |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Méthodes

| Nom | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ReferredArea) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ReferredArea, IComparer&lt;ReferredArea&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ReferredArea, IComparer&lt;ReferredArea&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ReferredArea) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ReferredArea[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ReferredArea[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ReferredArea[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ReferredArea&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ReferredArea&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ReferredArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ReferredArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ReferredArea&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ReferredArea&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ReferredArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ReferredArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ReferredArea&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ReferredArea&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ReferredArea) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ReferredArea, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ReferredArea, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ReferredArea) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ReferredArea, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ReferredArea, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Exemples

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassReferredAreaCollectionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Définissez des valeurs dans les cellules A2:C3 qui seront référencées par E1
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(2);
            worksheet.Cells["C2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(4);
            worksheet.Cells["B3"].PutValue(5);
            worksheet.Cells["C3"].PutValue(6);

            // Créez une formule dans E1 qui référence A2:C3
            worksheet.Cells["E1"].Formula = "=SUM(A2:C3)";

            // Obtenez les antécédents de E1
            ReferredAreaCollection referredAreas = worksheet.Cells["E1"].GetPrecedents();

            if (referredAreas != null)
            {
                foreach (ReferredArea area in referredAreas)
                {
                    StringBuilder sb = new StringBuilder();
                    if (area.IsExternalLink)
                    {
                        sb.Append("[");
                        sb.Append(area.ExternalFileName);
                        sb.Append("]");
                    }
                    sb.Append(area.SheetName);
                    sb.Append("!");
                    sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                    if (area.IsArea)
                    {
                        sb.Append(":");
                        sb.Append(CellsHelper.CellIndexToName(area.EndRow, area.EndColumn));
                    }
                    Console.WriteLine("Referred area: " + sb.ToString());
                }
            }
        }
    }
}
```

### Voir aussi

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ReferredArea](../referredarea/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


