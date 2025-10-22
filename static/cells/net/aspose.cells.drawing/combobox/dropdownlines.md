##ComboBox.DropDownLines
ComboBox property. Gets or sets the number of list lines displayed in the dropdown portion of a combo box
## ComboBox.DropDownLines property
Gets or sets the number of list lines displayed in the drop-down portion of a combo box.
```csharp
public int DropDownLines { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxPropertyDropDownLinesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a ComboBox with correct parameters
ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 0, 0, 100, 100);
comboBox.DropDownLines = 5;
// Populate worksheet cells with items
worksheet.Cells["A1"].PutValue("Item 1");
worksheet.Cells["A2"].PutValue("Item 2");
worksheet.Cells["A3"].PutValue("Item 3");
worksheet.Cells["A4"].PutValue("Item 4");
worksheet.Cells["A5"].PutValue("Item 5");
worksheet.Cells["A6"].PutValue("Item 6");
// Link combo box to cell values
comboBox.InputRange = "A1:A6";
workbook.Save("ComboBoxDropDownLinesDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
