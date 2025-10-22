##OleObject.ClassIdentifier
OleObject property. Gets and sets the class identifier of the embedded object. It means which application opens the embedded file
## OleObject.ClassIdentifier property
Gets and sets the class identifier of the embedded object. It means which application opens the embedded file.
```csharp
public byte[] ClassIdentifier { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertyClassIdentifierDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Sample byte array for ClassIdentifier (normally this would be a real class ID)
byte[] classId = new byte[] { 0x01, 0x02, 0x03, 0x04, 0x05, 0x06, 0x07, 0x08,
0x09, 0x0A, 0x0B, 0x0C, 0x0D, 0x0E, 0x0F, 0x10 };
// Add an OLE object with sample data
int oleIndex = sheet.OleObjects.Add(10, 10, 200, 100, new byte[100]);
OleObject oleObject = sheet.OleObjects[oleIndex];
// Set the ClassIdentifier property
oleObject.ClassIdentifier = classId;
oleObject.ProgID = "Excel.Sheet.12";
oleObject.DisplayAsIcon = true;
// Save the workbook
workbook.Save("OleObjectDemo.xlsx");
// Load the saved workbook to verify the ClassIdentifier
Workbook loadedWorkbook = new Workbook("OleObjectDemo.xlsx");
OleObject loadedOle = loadedWorkbook.Worksheets[0].OleObjects[0];
// Verify the ClassIdentifier was preserved
Console.WriteLine("ClassIdentifier length: " + loadedOle.ClassIdentifier.Length);
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
