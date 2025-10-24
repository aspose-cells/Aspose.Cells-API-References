##OleObject.IsLink
OleObject property. Returns true if the OleObject links to the file
## OleObject.IsLink property
Returns true if the OleObject links to the file.
```csharp
public bool IsLink { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OleObjectPropertyIsLinkDemo
{
public static void Run()
{
// Load the source workbook
Workbook workbook = new Workbook("example.xlsm");
// Process each worksheet
foreach (Worksheet worksheet in workbook.Worksheets)
{
// Process each OLE object in the worksheet
foreach (Aspose.Cells.Drawing.OleObject ole in worksheet.OleObjects)
{
// Skip if the OLE object is not linked
if (!ole.IsLink)
{
Console.WriteLine("Skipping embedded OLE object");
continue;
}
// Display and modify the linked file path
Console.WriteLine("Original linked file: " + ole.ObjectSourceFullName);
string newPath = ole.ObjectSourceFullName.Replace("C:", "D:");
ole.ObjectSourceFullName = newPath;
Console.WriteLine("Modified linked file: " + ole.ObjectSourceFullName);
}
}
// Save the modified workbook
workbook.Save("modified_example.xlsm");
Console.WriteLine("File saved with updated OLE links.");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
