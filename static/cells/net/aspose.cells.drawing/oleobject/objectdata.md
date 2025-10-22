##OleObject.ObjectData
OleObject property. Represents embedded ole object data as byte array
## OleObject.ObjectData property
Represents embedded ole object data as byte array.
```csharp
public byte[] ObjectData { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OleObjectPropertyObjectDataDemo
{
public static void Run()
{
// Create a new workbook
var workbook = new Workbook();
// Access first worksheet
var worksheet = workbook.Worksheets[0];
// Sample file paths (replace with actual paths in your environment)
string imagePath = "logo.jpg";
string oleDataPath = "test.xls";
// Add OLE object with initial image data
int oleIndex = worksheet.OleObjects.Add(10, 10, 300, 200, File.ReadAllBytes(imagePath));
// Modify the OLE object's data
worksheet.OleObjects[oleIndex].ObjectData = File.ReadAllBytes(oleDataPath);
// Save the workbook
workbook.Save("OleObjectDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("OLE object demo created successfully.");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
