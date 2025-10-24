##ListBox.Shadow
ListBox property. Indicates whether the combobox has 3D shading
## ListBox.Shadow property
Indicates whether the combobox has 3-D shading.
```csharp
public bool Shadow { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ListBoxPropertyShadowDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate list items
worksheet.Cells["A1"].PutValue("Option 1");
worksheet.Cells["A2"].PutValue("Option 2");
worksheet.Cells["A3"].PutValue("Option 3");
// Create listbox and set core properties
ListBox listBox = worksheet.Shapes.AddListBox(2, 1, 5, 1, 100, 150);
listBox.InputRange = "A1:A3";
listBox.LinkedCell = "B1";
// Set shadow property
listBox.Shadow = true;
// Save and reload to verify
workbook.Save("ListBoxShadowDemo.xlsx");
Workbook loadedWorkbook = new Workbook("ListBoxShadowDemo.xlsx");
ListBox loadedBox = (ListBox)loadedWorkbook.Worksheets[0].Shapes[0];
Console.WriteLine("Shadow enabled: " + loadedBox.Shadow);
}
}
}
```
### See Also
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
