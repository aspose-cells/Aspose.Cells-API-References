##Worksheet.TextBoxes
Worksheet property. Gets a TextBox collection
## Worksheet.TextBoxes property
Gets a [`TextBox`](../../../aspose.cells.drawing/textbox/) collection.
```csharp
public TextBoxCollection TextBoxes { get; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class WorksheetPropertyTextBoxesDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add a text box to the worksheet
int tID = ws.TextBoxes.Add(1, 1, 500, 1000);
Aspose.Cells.Drawing.TextBox textBox = ws.TextBoxes[tID];
// Set text and format parts of it
textBox.Text = "Red text 1. Plain text 1. Red text 2. Plain text 2.";
textBox.Characters(0, 10).Font.Color = Color.Red;
textBox.Characters(26, 10).Font.Color = Color.DarkRed;
// Save the workbook
wb.Save("TextBoxExample.xlsx");
}
}
}
```
### See Also
* class [TextBoxCollection](../../../aspose.cells.drawing/textboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
