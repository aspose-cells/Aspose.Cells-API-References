##ComboBox.SelectedValue
ComboBox property. Gets the selected value of the combox box
## ComboBox.SelectedValue property
Gets the selected value of the combox box.
```csharp
public string SelectedValue { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ComboBoxPropertySelectedValueDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a ComboBox and add items
Aspose.Cells.Drawing.ComboBox comboBox = (Aspose.Cells.Drawing.ComboBox)worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 50);
comboBox.LinkedCell = "A1";
comboBox.SetInputRange("B1:B4", false, false);
// Set values in the input range
worksheet.Cells["B1"].PutValue("a");
worksheet.Cells["B2"].PutValue("b");
worksheet.Cells["B3"].PutValue("c");
worksheet.Cells["B4"].PutValue("d");
// Demonstrate SelectedValue (read-only property)
Console.WriteLine("SelectedValue: " + comboBox.SelectedValue);
// Save the workbook
workbook.Save("ComboBoxDemo.xlsx");
}
}
}
```
### See Also
* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
