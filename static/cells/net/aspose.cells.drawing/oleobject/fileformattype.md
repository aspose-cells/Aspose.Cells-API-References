##OleObject.FileFormatType
OleObject property. Gets and sets the file type of the embedded ole object data
## OleObject.FileFormatType property
Gets and sets the file type of the embedded ole object data
```csharp
public FileFormatType FileFormatType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertyFileFormatTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add an OLE object to the worksheet (without file data)
int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, null);
// Get the added OLE object
OleObject oleObject = worksheet.OleObjects[oleIndex];
// Set and display the file format type
oleObject.FileFormatType = FileFormatType.Docm;
Console.WriteLine("OLE Object File Format Type: " + oleObject.FileFormatType);
// Save the workbook
workbook.Save("OleObjectFileFormatTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FileFormatType](../../../aspose.cells/fileformattype/)
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
