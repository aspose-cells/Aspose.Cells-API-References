##DxfCollection.Item
DxfCollection property. Gets the element at the specified index
## DxfCollection indexer
Gets the element at the specified index.
```csharp
public Style this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The specified index. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DxfCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the DxfCollection from the workbook
DxfCollection dxfCollection = workbook.Worksheets.Dxfs;
// Create a new style (can't add directly to DxfCollection as it has no Add method)
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 12;
// Style is automatically added to collection when created
// Get the first item from DxfCollection using Item property
Style firstStyle = dxfCollection[0];
Console.WriteLine("First style font name: " + firstStyle.Font.Name);
// Modify the style through the Item property (since it returns a reference)
firstStyle.Font.Color = System.Drawing.Color.Red;
firstStyle.Font.IsBold = true;
// Verify the change
Console.WriteLine("Modified style font color: " + dxfCollection[0].Font.Color);
Console.WriteLine("Modified style font bold: " + dxfCollection[0].Font.IsBold);
// Apply the style to a cell to see the effect
worksheet.Cells["A1"].PutValue("DxfCollection Property Item Demo");
worksheet.Cells["A1"].SetStyle(dxfCollection[0]);
// Save the result
workbook.Save("DxfCollectionPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [DxfCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
