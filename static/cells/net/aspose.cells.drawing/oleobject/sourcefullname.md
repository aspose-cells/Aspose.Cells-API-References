##OleObject.SourceFullName
OleObject property. Returns the source full name of the source file for the linked OLE object
## OleObject.SourceFullName property
Returns the source full name of the source file for the linked OLE object.
```csharp
[Obsolete("Use OleObject.ObjectSourceFullName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string SourceFullName { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use OleObject.ObjectSourceFullName property. This property will be removed 12 months later since November 2013. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertySourceFullNameDemo
{
public static void Run()
{
// Load the sample Excel file with OLE objects
Workbook workbook = new Workbook("TEST_OLE_Book1.xlsx");
// Get the first worksheet's OLE objects collection
OleObjectCollection oleObjects = workbook.Worksheets[0].OleObjects;
// Process each OLE object
foreach (OleObject oleObject in oleObjects)
{
// Demonstrate SourceFullName property usage
Console.WriteLine($"OLE Object Source: {oleObject.SourceFullName}");
// Create a file using the SourceFullName and write OLE data
using (FileStream stream = new FileStream(oleObject.SourceFullName, FileMode.Create, FileAccess.Write))
{
stream.Write(oleObject.ObjectData, 0, oleObject.ObjectData.Length);
}
}
// Save the modified workbook
workbook.Save("TEST_OLE_Book1_out.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
