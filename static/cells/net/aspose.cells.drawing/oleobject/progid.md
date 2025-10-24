##OleObject.ProgID
OleObject property. Gets or sets the ProgID of the OLE object
## OleObject.ProgID property
Gets or sets the ProgID of the OLE object.
```csharp
public string ProgID { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertyProgIDDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an OLE object to the worksheet
int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0], "test.pdf");
OleObject ole = worksheet.OleObjects[oleIndex];
// Set the ProgID for the OLE object
ole.ProgID = "AcroExch.Document.DC";
// Display the ProgID
Console.WriteLine("OLE Object ProgID: " + ole.ProgID);
// Save the workbook
workbook.Save("OleObjectProgIDDemo.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
