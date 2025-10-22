##OleObject.IsAutoSize
OleObject property. True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated
## OleObject.IsAutoSize property
True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.
```csharp
public bool IsAutoSize { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertyIsAutoSizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an OLE object (using file data as byte array)
byte[] oleData = System.IO.File.ReadAllBytes(@"C:\example\test.docx");
int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, oleData);
Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];
// Set and demonstrate IsAutoSize property
oleObject.IsAutoSize = true;
Console.WriteLine("OLE Object AutoSize initially: " + oleObject.IsAutoSize);
// Change the property
oleObject.IsAutoSize = false;
Console.WriteLine("OLE Object AutoSize after change: " + oleObject.IsAutoSize);
// Save the workbook
workbook.Save("OleObjectIsAutoSizeDemo.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
