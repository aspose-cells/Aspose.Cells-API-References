---
title: Class SmartTagCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Markup.SmartTagCollection class. Represents all smart tags in the cell
type: docs
url: /net/aspose.cells.markup/smarttagcollection/
---
## SmartTagCollection class

Represents all smart tags in the cell.

```csharp
public class SmartTagCollection : CollectionBase<SmartTag>
```

## Properties

| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Column](../../aspose.cells.markup/smarttagcollection/column/) { get; } | Gets the column of the cell smart tags. |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.markup/smarttagcollection/item/) { get; } | Gets a [`SmartTag`](../smarttag/) object at the specific index |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
| [Row](../../aspose.cells.markup/smarttagcollection/row/) { get; } | Gets the row of the cell smart tags. |

## Methods

| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagcollection/add/)(string, string) | Adds a smart tag. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SmartTag) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SmartTag, IComparer&lt;SmartTag&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, SmartTag, IComparer&lt;SmartTag&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(SmartTag) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SmartTag[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SmartTag[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, SmartTag[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;SmartTag&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;SmartTag&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;SmartTag&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;SmartTag&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;SmartTag&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;SmartTag&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;SmartTag&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;SmartTag&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;SmartTag&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;SmartTag&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SmartTag) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SmartTag, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SmartTag, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SmartTag) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SmartTag, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SmartTag, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |

### Examples

```csharp
// Called: SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
public static void Type_SmartTagCollection()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Add some sample data
            sheet.Cells[&quot;A1&quot;].PutValue(&quot;Aspose&quot;);
            sheet.Cells[&quot;A2&quot;].PutValue(&quot;Cells&quot;);

            // Access the SmartTagSetting of the worksheet
            SmartTagSetting smartTagSetting = sheet.SmartTagSetting;

            // Add a smart tag to cell A1
            int smartTagIndex = smartTagSetting.Add(0, 0); // A1 is at row 0, column 0
            SmartTagCollection smartTags = smartTagSetting[smartTagIndex];

            // Add properties to the smart tag
            smartTags.Add(&quot;http://docs.aspose.com&quot;, &quot;docs&quot;);
            SmartTag smartTag = smartTags[0];
            smartTag.SetLink(&quot;http://www.aspose.com&quot;, &quot;AsposeLink&quot;);

            // Add properties to the smart tag
            SmartTagPropertyCollection properties = smartTag.Properties;
            properties.Add(&quot;Author&quot;, &quot;Aspose&quot;);
            properties.Add(&quot;Description&quot;, &quot;Aspose.Cells SmartTag&quot;);

            // Save the workbook
            workbook.Save(&quot;SmartTagPropertyDemo.xlsx&quot;);

            Console.WriteLine(&quot;SmartTagPropertyDemo.xlsx created successfully.&quot;);
        }
```

### See Also

* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [SmartTag](../smarttag/)
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


