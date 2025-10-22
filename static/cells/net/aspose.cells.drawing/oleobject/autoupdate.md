##OleObject.AutoUpdate
OleObject property. Specifies whether the link to the OleObject is automatically updated or not
## OleObject.AutoUpdate property
Specifies whether the link to the OleObject is automatically updated or not.
```csharp
public bool AutoUpdate { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertyAutoUpdateDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample files for demonstration
string imagePath = "OleObjectExample.jpg";
string excelPath = "OleObjectExample.xls";
// Create sample image file if it doesn't exist
if (!File.Exists(imagePath))
{
using (File.Create(imagePath)) { }
}
// Create sample Excel file if it doesn't exist
if (!File.Exists(excelPath))
{
new Workbook().Save(excelPath);
}
// Read image data
byte[] imageData = File.ReadAllBytes(imagePath);
// Add OleObject to worksheet
int oleIndex = sheet.OleObjects.Add(1, 1, 200, 200, imageData);
Aspose.Cells.Drawing.OleObject oleObject = sheet.OleObjects[oleIndex];
// Set OleObject properties
oleObject.ObjectData = File.ReadAllBytes(excelPath);
oleObject.ProgID = "Excel.Sheet.8";
oleObject.DisplayAsIcon = true;
// Demonstrate AutoUpdate property
oleObject.AutoUpdate = false; // When false, the object won't update automatically when source changes
// Save the workbook
workbook.Save("OleObjectAutoUpdateDemo.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
