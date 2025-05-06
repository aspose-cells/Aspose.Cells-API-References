---
title: Class CustomFilterCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CustomFilterCollection class. Represents the custom filters
type: docs
url: /net/aspose.cells/customfiltercollection/
---
## CustomFilterCollection class

Represents the custom filters.

```csharp
public class CustomFilterCollection : CollectionBase<CustomFilter>
```

## Constructors

| Name | Description |
| --- | --- |
| [CustomFilterCollection](customfiltercollection/)() | Constructs new instance. |

## Properties

| Name | Description |
| --- | --- |
| [And](../../aspose.cells/customfiltercollection/and/) { get; set; } | Indicates whether the two criteria have an "and" relationship. |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells/customfiltercollection/item/) { get; } | Gets the custom filter in the specific index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |

## Methods

| Name | Description |
| --- | --- |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomFilter) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CustomFilter, IComparer&lt;CustomFilter&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CustomFilter, IComparer&lt;CustomFilter&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CustomFilter) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomFilter[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CustomFilter[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CustomFilter[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CustomFilter&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CustomFilter&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CustomFilter&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CustomFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CustomFilter&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CustomFilter&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomFilter) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomFilter, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CustomFilter, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomFilter) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomFilter, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CustomFilter, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
// Called: CustomFilterCollection customFilters = new CustomFilterCollection();
public static void Type_CustomFilterCollection()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Apple&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;Banana&quot;);
            sheet.Cells[&quot;A3&quot;].PutValue(&quot;Cherry&quot;);
            sheet.Cells[&quot;A4&quot;].PutValue(&quot;Date&quot;);
            sheet.Cells[&quot;A5&quot;].PutValue(&quot;Elderberry&quot;);

            // Create a CustomFilterCollection
            CustomFilterCollection customFilters = new CustomFilterCollection();

            //// Create a CustomFilter for filtering fruits that start with &apos;A&apos; or &apos;B&apos;
            //CustomFilter filter1 = new CustomFilter()
            //{
            //    FilterOperatorType = FilterOperatorType.Equal,
            //    Criteria = &quot;Apple&quot;
            //};

            //CustomFilter filter2 = new CustomFilter()
            //{
            //    FilterOperatorType = FilterOperatorType.Equal,
            //    Criteria = &quot;Banana&quot;
            //};

            //// Add filters to the collection with &quot;And&quot; relationship
            //customFilters.And = true;

            //// Set criteria for the filters
            //customFilters.Append(filter1);
            //customFilters.Append(filter2);

            // Apply the custom filters to the worksheet
            // Assuming we have a method to apply filters (not defined in the provided code)
            ApplyCustomFilters(sheet, customFilters);

            // Save the workbook
            workbook.Save(&quot;CustomFilterDemo.xlsx&quot;);
            workbook.Save(&quot;CustomFilterDemo.pdf&quot;);
        }
```

### See Also

* class [CollectionBase&lt;T&gt;](../collectionbase-1/)
* class [CustomFilter](../customfilter/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


