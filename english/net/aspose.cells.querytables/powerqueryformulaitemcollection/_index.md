---
title: Class PowerQueryFormulaItemCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.QueryTables.PowerQueryFormulaItemCollection class. Represents all item of the power query formula
type: docs
url: /net/aspose.cells.querytables/powerqueryformulaitemcollection/
---
## PowerQueryFormulaItemCollection class

Represents all item of the power query formula.

```csharp
public class PowerQueryFormulaItemCollection : CollectionBase<PowerQueryFormulaItem>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.querytables/powerqueryformulaitemcollection/item/) { get; } | Gets [`PowerQueryFormulaItem`](../powerqueryformulaitem/) by the index in the list. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormulaItem) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(PowerQueryFormulaItem, IComparer&lt;PowerQueryFormulaItem&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, PowerQueryFormulaItem, IComparer&lt;PowerQueryFormulaItem&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(PowerQueryFormulaItem) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormulaItem[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(PowerQueryFormulaItem[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, PowerQueryFormulaItem[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;PowerQueryFormulaItem&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormulaItem) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormulaItem, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(PowerQueryFormulaItem, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormulaItem) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormulaItem, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(PowerQueryFormulaItem, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
// Called: PowerQueryFormulaItemCollection PQFIcoll = PQF.PowerQueryFormulaItems;
[Test]
        public void Type_PowerQueryFormulaItemCollection()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava43073.xlsm");

            PowerQueryFormulaCollection PQFcoll = workbook.DataMashup.PowerQueryFormulas;//Exception here
            Assert.AreEqual(PQFcoll.Count, 2);

            PowerQueryFormula PQF = PQFcoll[1];
            Assert.AreEqual("Change Management", PQF.Name);
            PowerQueryFormulaItemCollection PQFIcoll = PQF.PowerQueryFormulaItems;
            Assert.AreEqual(3, PQFIcoll.Count);

            PowerQueryFormulaItem PQFI = PQFIcoll[0];
            Assert.AreEqual("Source", PQFI.Name);
            Assert.AreEqual(PQFI.Value, "SharePoint.Tables(\"https://cimconuso.sharepoint.com\", [ApiVersion = 15])");

            workbook.Save(Constants.destPath + "CellsJava43073.xlsm");

        }
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [PowerQueryFormulaItem](../powerqueryformulaitem/)
* namespace [Aspose.Cells.QueryTables](../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../)


