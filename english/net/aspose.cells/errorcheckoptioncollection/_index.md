---
title: Class ErrorCheckOptionCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ErrorCheckOptionCollection class. Represents all error check option
type: docs
url: /net/aspose.cells/errorcheckoptioncollection/
---
## ErrorCheckOptionCollection class

Represents all error check option.

```csharp
public class ErrorCheckOptionCollection : CollectionBase<ErrorCheckOption>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/errorcheckoptioncollection/item/) { get; } | Gets [`ErrorCheckOption`](../errorcheckoption/) object by the given index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/errorcheckoptioncollection/add/)() | Add an error check option. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ErrorCheckOption) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(ErrorCheckOption, IComparer&lt;ErrorCheckOption&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, ErrorCheckOption, IComparer&lt;ErrorCheckOption&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(ErrorCheckOption) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ErrorCheckOption[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(ErrorCheckOption[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, ErrorCheckOption[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;ErrorCheckOption&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;ErrorCheckOption&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ErrorCheckOption) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ErrorCheckOption, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(ErrorCheckOption, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ErrorCheckOption) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ErrorCheckOption, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(ErrorCheckOption, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
// Called: ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;
public static void Type_ErrorCheckOptionCollection()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Get the ErrorCheckOptionCollection from the worksheet
            ErrorCheckOptionCollection opts = worksheet.ErrorCheckOptions;

            // Add a new ErrorCheckOption to the collection
            int optionIdx = opts.Add();
            ErrorCheckOption opt = opts[optionIdx];

            // Set error check options
            opt.SetErrorCheck(ErrorCheckType.InconsistFormula, false);
            opt.SetErrorCheck(ErrorCheckType.InconsistRange, false);
            opt.SetErrorCheck(ErrorCheckType.TextDate, false);
            opt.SetErrorCheck(ErrorCheckType.TextNumber, false);
            opt.SetErrorCheck(ErrorCheckType.Validation, false);

            // Define a cell area and add it to the ErrorCheckOption
            CellArea ca = CellArea.CreateCellArea("A1", "B10");
            opt.AddRange(ca);

            // Save the workbook
            workbook.Save("ErrorCheckOptionExample.xlsx");
            workbook.Save("ErrorCheckOptionExample.pdf");
        }
```

### See Also

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ErrorCheckOption](../errorcheckoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


