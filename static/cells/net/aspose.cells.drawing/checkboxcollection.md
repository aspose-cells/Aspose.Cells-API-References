##Class CheckBoxCollection
Aspose.Cells.Drawing.CheckBoxCollection class. Represents a collection of CheckBox objects in a worksheet
## CheckBoxCollection class
Represents a collection of [`CheckBox`](../checkbox/) objects in a worksheet.
```csharp
public class CheckBoxCollection : CollectionBase<CheckBox>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/checkboxcollection/item/) { get; } | Gets the [`CheckBox`](../checkbox/) element at the specified index. |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.drawing/checkboxcollection/add/)(int, int, int, int) | Adds a checkBox to the collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CheckBox) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(CheckBox, IComparer&lt;CheckBox&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, CheckBox, IComparer&lt;CheckBox&gt;) |  |
| [Clear](../../aspose.cells/collectionbase-1/clear/)() |  |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(CheckBox) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CheckBox[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(CheckBox[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, CheckBox[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;CheckBox&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;CheckBox&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;CheckBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;CheckBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;CheckBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;CheckBox&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;CheckBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;CheckBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;CheckBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;CheckBox&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CheckBox) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CheckBox, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(CheckBox, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CheckBox) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CheckBox, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(CheckBox, int, int) |  |
| [RemoveAt](../../aspose.cells/collectionbase-1/removeat/)(int) |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class CheckBoxCollectionDemo
{
public static void CheckBoxCollectionExample()
{
// Create a new Workbook.
Workbook workbook = new Workbook();
// Get the first worksheet in the workbook.
Worksheet sheet = workbook.Worksheets[0];
// Add a CheckBox to the worksheet.
int index = sheet.CheckBoxes.Add(15, 15, 20, 100);
CheckBox checkBox = sheet.CheckBoxes[index];
checkBox.Text = "Check Box 1";
// Save the workbook.
workbook.Save("CheckBoxCollectionExample.xlsx");
workbook.Save("CheckBoxCollectionExample.pdf");
return;
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [CheckBox](../checkbox/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
