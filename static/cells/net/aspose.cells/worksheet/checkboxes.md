##Worksheet.CheckBoxes
Worksheet property. Gets a CheckBox collection
## Worksheet.CheckBoxes property
Gets a [`CheckBox`](../../../aspose.cells.drawing/checkbox/) collection.
```csharp
public CheckBoxCollection CheckBoxes { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class WorksheetPropertyCheckBoxesDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add three checkboxes with different properties
int index1 = sheet.CheckBoxes.Add(10, 10, 20, 100);
Aspose.Cells.Drawing.CheckBox checkBox1 = sheet.CheckBoxes[index1];
checkBox1.Text = "Option 1";
checkBox1.Value = true;
int index2 = sheet.CheckBoxes.Add(40, 10, 20, 100);
Aspose.Cells.Drawing.CheckBox checkBox2 = sheet.CheckBoxes[index2];
checkBox2.Text = "Option 2";
checkBox2.LinkedCell = "A1";
int index3 = sheet.CheckBoxes.Add(70, 10, 20, 100);
Aspose.Cells.Drawing.CheckBox checkBox3 = sheet.CheckBoxes[index3];
checkBox3.Text = "Option 3";
checkBox3.Value = true;
workbook.Save("CheckBoxesDemo.xlsx");
}
}
}
```
### See Also
* class [CheckBoxCollection](../../../aspose.cells.drawing/checkboxcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
