##Class TextBoxCollection
Aspose.Cells.Drawing.TextBoxCollection class. Encapsulates a collection of TextBox objects
## TextBoxCollection class
Encapsulates a collection of [`TextBox`](../textbox/) objects.
```csharp
public class TextBoxCollection : CollectionBase<TextBox>
```
## Properties
| Name | Description |
| --- | --- |
| [Capacity](../../aspose.cells/collectionbase-1/capacity/) { get; set; } |  |
| [Count](../../aspose.cells/collectionbase-1/count/) { get; } |  |
| [Item](../../aspose.cells.drawing/textboxcollection/item/) { get; } | Gets the [`TextBox`](../textbox/) element at the specified index. (2 indexers) |
| [Item](../../aspose.cells/collectionbase-1/item/) { get; set; } |  |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells.drawing/textboxcollection/add/)(int, int, int, int) | Adds a textbox to the collection. |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextBox) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(TextBox, IComparer&lt;TextBox&gt;) |  |
| [BinarySearch](../../aspose.cells/collectionbase-1/binarysearch/)(int, int, TextBox, IComparer&lt;TextBox&gt;) |  |
| [Clear](../../aspose.cells.drawing/textboxcollection/clear/#clear)() | Clear all text boxes. (2 methods) |
| [Contains](../../aspose.cells/collectionbase-1/contains/)(TextBox) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TextBox[]) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(TextBox[], int) |  |
| [CopyTo](../../aspose.cells/collectionbase-1/copyto/)(int, TextBox[], int, int) |  |
| [Exists](../../aspose.cells/collectionbase-1/exists/)(Predicate&lt;TextBox&gt;) |  |
| [Find](../../aspose.cells/collectionbase-1/find/)(Predicate&lt;TextBox&gt;) |  |
| [FindAll](../../aspose.cells/collectionbase-1/findall/)(Predicate&lt;TextBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(Predicate&lt;TextBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, Predicate&lt;TextBox&gt;) |  |
| [FindIndex](../../aspose.cells/collectionbase-1/findindex/)(int, int, Predicate&lt;TextBox&gt;) |  |
| [FindLast](../../aspose.cells/collectionbase-1/findlast/)(Predicate&lt;TextBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(Predicate&lt;TextBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, Predicate&lt;TextBox&gt;) |  |
| [FindLastIndex](../../aspose.cells/collectionbase-1/findlastindex/)(int, int, Predicate&lt;TextBox&gt;) |  |
| [GetEnumerator](../../aspose.cells/collectionbase-1/getenumerator/)() |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TextBox) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TextBox, int) |  |
| [IndexOf](../../aspose.cells/collectionbase-1/indexof/)(TextBox, int, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TextBox) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TextBox, int) |  |
| [LastIndexOf](../../aspose.cells/collectionbase-1/lastindexof/)(TextBox, int, int) |  |
| [RemoveAt](../../aspose.cells.drawing/textboxcollection/removeat/#removeat)(int) | Remove a text box from the file. (2 methods) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class TextBoxCollectionDemo
{
public static void TextBoxCollectionExample()
{
// Instantiating a Workbook object
Workbook workbook = new Workbook();
// Get the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Get the TextBoxCollection object
TextBoxCollection textBoxCollection = worksheet.TextBoxes;
// Add a TextBox to the collection
int textBoxIndex = textBoxCollection.Add(1, 1, 50, 100);
// Access the added TextBox
TextBox textBox = textBoxCollection[textBoxIndex];
// Set some properties of the TextBox
textBox.Text = "Hello, Aspose!";
textBox.Font.Name = "Arial";
textBox.Font.Size = 12;
textBox.Font.IsBold = true;
// Iterate through all TextBoxes in the collection
foreach (TextBox tbox in textBoxCollection)
{
// Perform operations on each TextBox
Console.WriteLine(tbox.Text);
}
// Save the workbook
workbook.Save("TextBoxCollectionExample.xlsx");
}
}
}
```
### See Also
* class [CollectionBase&lt;T&gt;](../../aspose.cells/collectionbase-1/)
* class [TextBox](../textbox/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
