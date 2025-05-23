---
title: Class ReferredAreaCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ReferredAreaCollection class. Represents all referred cells and areas
type: docs
url: /net/aspose.cells/referredareacollection/
---
## ReferredAreaCollection class

Represents all referred cells and areas.

```csharp
public class ReferredAreaCollection : CollectionBase<ReferredArea>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/referredareacollection/item/) { get; } |  |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
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

### Examples

```csharp
// Called: ReferredAreaCollection ret = workbook.Worksheets[0].Cells["E1"].GetPrecedents();
public void Cells_Type_ReferredAreaCollection()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    ReferredAreaCollection ret = workbook.Worksheets[0].Cells["E1"].GetPrecedents();
    if (ret != null)
    {
        for (int m = 0; m < ret.Count; m++)
        {
            ReferredArea area = ret[m];
            StringBuilder stringBuilder = new StringBuilder();
            if (area.IsExternalLink)
            {
                stringBuilder.Append("[");
                stringBuilder.Append(area.ExternalFileName);
                stringBuilder.Append("]");
            }
            stringBuilder.Append(area.SheetName);
            stringBuilder.Append("!");
            stringBuilder.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
            if (area.IsArea)
            {
                stringBuilder.Append(":");
                stringBuilder.Append(CellsHelper.CellIndexToName(area.EndRow, area.EndColumn));
            }
            Assert.AreEqual(stringBuilder.ToString(), "Sheet1!A2:C3");
        }
    }
}
```

### See Also

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ReferredArea](../referredarea/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


