##ComboBox.SelectedIndex
ComboBox property. Gets or sets the index number of the currently selected item in a list box or combo box. Zerobased
## ComboBox.SelectedIndex property
Gets or sets the index number of the currently selected item in a list box or combo box. Zero-based.
```csharp
public int SelectedIndex { get; set; }
```
### Remarks
-1 presents no item is selected.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxPropertySelectedIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the combo box
worksheet.Cells["A1"].PutValue("Item 1");
worksheet.Cells["A2"].PutValue("Item 2");
worksheet.Cells["A3"].PutValue("Item 3");
worksheet.Cells["A4"].PutValue("Item 4");
worksheet.Cells["A5"].PutValue("Item 5");
// Add a combo box to the worksheet
Shape shape = worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 20);
ComboBox comboBox = (ComboBox)shape;
// Set the input range for the combo box
comboBox.InputRange = "A1:A5";
comboBox.DropDownLines = 5;
// Set and display the selected index
comboBox.SelectedIndex = 2; // Selects "Item 3" (zero-based index)
Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
Console.WriteLine("Selected Value: " + comboBox.SelectedValue);
// Change the selected index and display again
comboBox.SelectedIndex = 4; // Selects "Item 5"
Console.WriteLine("\nAfter changing selection:");
Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
Console.WriteLine("Selected Value: " + comboBox.SelectedValue);
}
}
}
```
### See Also
* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
