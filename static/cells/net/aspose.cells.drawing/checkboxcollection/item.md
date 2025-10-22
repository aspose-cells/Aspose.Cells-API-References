##CheckBoxCollection.Item
CheckBoxCollection property. Gets the CheckBox element at the specified index
## CheckBoxCollection indexer
Gets the [`CheckBox`](../../checkbox/) element at the specified index.
```csharp
public CheckBox this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class CheckBoxCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a checkbox to the worksheet
int index = worksheet.CheckBoxes.Add(10, 10, 100, 20);
// Access the checkbox using Item property (indexer)
Aspose.Cells.Drawing.CheckBox checkBox = worksheet.CheckBoxes[index];
checkBox.Text = "Sample CheckBox";
checkBox.Name = "CheckBox1";
// Access the checkbox using index (Item property)
Aspose.Cells.Drawing.CheckBox checkBoxByName = worksheet.CheckBoxes[0];
// Output the checkbox properties
Console.WriteLine("CheckBox Name: " + checkBoxByName.Name);
Console.WriteLine("CheckBox Text: " + checkBoxByName.Text);
// Save the workbook
workbook.Save("CheckBoxExample.xlsx");
}
}
}
```
### See Also
* class [CheckBox](../../checkbox/)
* class [CheckBoxCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
