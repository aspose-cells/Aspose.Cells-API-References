##Class SmartTagPropertyCollection
Aspose.Cells.Markup.SmartTagPropertyCollection class. Represents all properties of cell smart tag
## SmartTagPropertyCollection class
Represents all properties of cell smart tag.
```csharp
public class SmartTagPropertyCollection : CollectionBase<SmartTagProperty>
```
## Constructors
| Name | Description |
| --- | --- |
| [SmartTagPropertyCollection](smarttagpropertycollection/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.markup/smarttagpropertycollection/item/) { get; } | Gets a [`SmartTagProperty`](../smarttagproperty/) object. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagpropertycollection/add/)(string, string) | Adds a property of cell's smart tag. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SmartTagProperty) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(SmartTagProperty, IComparer&lt;SmartTagProperty&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, SmartTagProperty, IComparer&lt;SmartTagProperty&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(SmartTagProperty) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SmartTagProperty[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(SmartTagProperty[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, SmartTagProperty[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;SmartTagProperty&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;SmartTagProperty&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;SmartTagProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;SmartTagProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;SmartTagProperty&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;SmartTagProperty&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;SmartTagProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;SmartTagProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;SmartTagProperty&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;SmartTagProperty&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SmartTagProperty) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SmartTagProperty, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(SmartTagProperty, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SmartTagProperty) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SmartTagProperty, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(SmartTagProperty, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markup;
namespace AsposeCellsExamples
{
public class MarkupClassSmartTagPropertyCollectionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
SmartTagSetting smartTagSetting = sheet.SmartTagSetting;
int smartTagIndex = smartTagSetting.Add(0, 0);
SmartTagCollection smartTags = smartTagSetting[smartTagIndex];
smartTags.Add("http://docs.aspose.com", "docs");
SmartTag smartTag = smartTags[0];
SmartTagPropertyCollection properties = smartTag.Properties;
properties.Add("Author", "Aspose");
properties.Add("Version", "1.0");
workbook.Save("SmartTagPropertyCollectionDemo.xlsx");
Console.WriteLine("SmartTagPropertyCollectionDemo.xlsx created successfully.");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [SmartTagProperty](../smarttagproperty/)
* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)
