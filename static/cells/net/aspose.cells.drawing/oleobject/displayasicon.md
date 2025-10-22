##OleObject.DisplayAsIcon
OleObject property. True if the specified object is displayed as an icon and the image will not be auto changed
## OleObject.DisplayAsIcon property
True if the specified object is displayed as an icon and the image will not be auto changed.
```csharp
public bool DisplayAsIcon { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertyDisplayAsIconDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add an OLE object (PDF) to the worksheet
byte[] pdfData = File.ReadAllBytes("example.pdf");
int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, pdfData);
// Get the OLE object
Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleIndex];
oleObject.ProgID = "AcroExch.Document.DC";
// Demonstrate DisplayAsIcon property
oleObject.DisplayAsIcon = true; // Show as icon
// oleObject.DisplayAsIcon = false; // Show content if possible
// Save the workbook
workbook.Save("OleObjectDisplayAsIconDemo.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
