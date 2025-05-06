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
// Called: var prec = worksheet1.Cells[&amp;quot;A1&amp;quot;].GetPrecedents();
[Test]
        public void Type_ReferredAreaCollection()
        {
            Workbook wb = new Workbook();
            wb.Worksheets.Add(&quot;Sheet2&quot;);
            var worksheet1 = wb.Worksheets[&quot;Sheet1&quot;];
            // the named range 
            wb.Worksheets[&quot;Sheet2&quot;].Cells.CreateRange(&quot;E5:I6&quot;).Name = &quot;someNamedRange_1&quot;;
            worksheet1.Cells[&quot;A1&quot;].Formula = &quot;=SUM(someNamedRange_1)&quot;;
            var prec = worksheet1.Cells[&quot;A1&quot;].GetPrecedents();
            Assert.AreEqual(&quot;Sheet2&quot;, prec[0].SheetName);
        }
```

### See Also

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ReferredArea](../referredarea/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


