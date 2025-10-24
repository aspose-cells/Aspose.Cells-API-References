##ComboBox.SelectedCell
ComboBox property. Gets the selected cell in the input range of the combo box
## ComboBox.SelectedCell property
Gets the selected cell in the input range of the combo box.
```csharp
public Cell SelectedCell { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ComboBoxPropertySelectedCellDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate cells with sample data for combobox items
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("Cherry");
worksheet.Cells["A4"].PutValue("Date");
worksheet.Cells["A5"].PutValue("Fig");
// Create a ComboBox and set its properties
ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 100, 100, 5, 0);
comboBox.InputRange = "A1:A5";
comboBox.DropDownLines = 5;
// Set selection and demonstrate SelectedCell
comboBox.SelectedIndex = 2;
Cell selectedCell = comboBox.SelectedCell;
Console.WriteLine($"Initial Selected Cell Value: {selectedCell.StringValue}");
// Modify the selected cell's value
selectedCell.PutValue("Orange");
Console.WriteLine($"Updated Selected Cell Value: {selectedCell.StringValue}");
// Show the effect on adjacent cells
worksheet.Cells["B3"].PutValue($"Combo Selection: {comboBox.SelectedValue}");
workbook.Save("ComboBoxSelectedCellDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../../aspose.cells/cell/)
* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
