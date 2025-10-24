##OleObject.AutoLoad
OleObject property. Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened
## OleObject.AutoLoad property
Specifies whether the host application for the embedded object shall be called to load the object data automatically when the parent workbook is opened.
```csharp
public bool AutoLoad { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertyAutoLoadDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add an OleObject to the worksheet
int oleNumber = sheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
// Set OleObject properties
OleObject ole = sheet.OleObjects[oleNumber];
ole.ProgID = "Excel.Sheet";
ole.ObjectData = new byte[0];
// Demonstrate AutoLoad property
ole.AutoLoad = true; // Automatically load the OleObject when the workbook opens
// Save the workbook
workbook.Save("OleObjectAutoLoadDemo.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
