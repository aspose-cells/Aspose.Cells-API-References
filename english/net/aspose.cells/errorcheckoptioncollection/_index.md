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
// Called: ErrorCheckOptionCollection optss = sheet.ErrorCheckOptions;
[Test]
        public void Type_ErrorCheckOptionCollection()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            ErrorCheckOptionCollection optss = sheet.ErrorCheckOptions;
            int index = optss.Add();
            ErrorCheckOption opts = optss[index];
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts.AddRange(CreateCellArea(&quot;A1&quot;, &quot;D2&quot;));
            opts.AddRange(CreateCellArea(&quot;A3&quot;, &quot;D3&quot;));
            index = optss.Add();
            opts = optss[index];
            opts.SetErrorCheck(ErrorCheckType.TwoDigitTextYear, false);
            opts.SetErrorCheck(ErrorCheckType.NumberStoredAsText, false);
            opts.AddRange(CreateCellArea(&quot;A3&quot;, &quot;D5&quot;));
            workbook.Save(Constants.destPath + &quot;TestErrorCheck.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;TestErrorCheck.xls&quot;);
            sheet = workbook.Worksheets[0];
            
            Assert.AreEqual(sheet.ErrorCheckOptions.Count, 2);
            opts = sheet.ErrorCheckOptions[0];
            Assert.AreEqual(opts.GetCountOfRange(), 2);
            Assert.AreEqual(opts.IsErrorCheck(ErrorCheckType.NumberStoredAsText), false);

        }
```

### See Also

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [ErrorCheckOption](../errorcheckoption/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


