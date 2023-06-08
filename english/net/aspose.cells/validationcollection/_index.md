---
title: Class ValidationCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ValidationCollection class. Represents data validation collection
type: docs
url: /net/aspose.cells/validationcollection/
---
## ValidationCollection class

Represents data validation collection.

```csharp
public class ValidationCollection : CollectionBase<Validation>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/validationcollection/item/) { get; } | Gets the [`Validation`](../validation/) element at the specified index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/validationcollection/add/#add)() | (**Obsolete.**) Adds a data validation to the collection. |
| [Add](../../aspose.cells/validationcollection/add/#add_1)(CellArea) | Adds a data validation to the collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Validation) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(Validation, IComparer&lt;Validation&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, Validation, IComparer&lt;Validation&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(Validation) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Validation[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(Validation[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, Validation[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;Validation&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;Validation&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;Validation&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;Validation&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;Validation&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;Validation&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;Validation&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;Validation&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;Validation&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;Validation&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [GetValidationInCell](../../aspose.cells/validationcollection/getvalidationincell/)(int, int) | Gets the validation applied to given cell. |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(Validation, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(Validation, int, int) |  |
| [RemoveACell](../../aspose.cells/validationcollection/removeacell/)(int, int) | Removes all validation setting on the cell. |
| [RemoveArea](../../aspose.cells/validationcollection/removearea/)(CellArea) | Removes all validation setting on the range.. |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
[C#]
Workbook workbook = new Workbook();
ValidationCollection validations = workbook.Worksheets[0].Validations;
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
Validation validation = validations[validations.Add(area)];
validation.Type = Aspose.Cells.ValidationType.List;
validation.Formula1 = "a,b,c,d";

[Visual Basic]
Dim workbook as Workbook = new Workbook()
Dim validations as ValidationCollection  = workbook.Worksheets(0).Validations
Dim area as CellArea = CellArea.CreateCellArea(0, 0, 1, 1);
Dim validation as Validation = validations(validations.Add(area))
validation.Type = ValidationType.List
validation.Formula1 = "a,b,c,d";
```

### See Also

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [Validation](../validation/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


