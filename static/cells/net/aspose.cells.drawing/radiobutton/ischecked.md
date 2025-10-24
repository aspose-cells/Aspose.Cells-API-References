##RadioButton.IsChecked
RadioButton property. Indicates if the radiobutton is checked or not
## RadioButton.IsChecked property
Indicates if the radiobutton is checked or not.
```csharp
public bool IsChecked { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class RadioButtonPropertyIsCheckedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a radio button to the worksheet
Shape shape = worksheet.Shapes.AddRadioButton(1, 0, 1, 0, 100, 100);
RadioButton radioButton = (RadioButton)shape;
// Set the radio button text
radioButton.Text = "Option 1";
// Initially unchecked
radioButton.IsChecked = false;
Console.WriteLine("Radio button initially unchecked: " + radioButton.IsChecked);
// Check the radio button
radioButton.IsChecked = true;
Console.WriteLine("Radio button after checking: " + radioButton.IsChecked);
// Save the workbook
workbook.Save("RadioButtonExample.xlsx");
}
}
}
```
### See Also
* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
