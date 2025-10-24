##OleObject.FullObjectBin
OleObject property. Gets the full embedded ole object binary data in the template file
## OleObject.FullObjectBin property
Gets the full embedded ole object binary data in the template file.
```csharp
public byte[] FullObjectBin { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class OleObjectPropertyFullObjectBinDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an OLE object to the worksheet
byte[] objectData = File.ReadAllBytes("example.docx");
int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, objectData, "docx");
OleObject oleObject = worksheet.OleObjects[oleObjectIndex];
// Set some properties for the OLE object
oleObject.FileFormatType = FileFormatType.Docx;
oleObject.ObjectData = objectData;
oleObject.IsAutoSize = true;
// Get the FullObjectBin data (read-only property)
byte[] fullObjectBinData = oleObject.FullObjectBin;
Console.WriteLine("FullObjectBin data length: " + (fullObjectBinData != null ? fullObjectBinData.Length.ToString() : "null"));
// Demonstrate usage of FullObjectBin by saving it to a file
if (fullObjectBinData != null && fullObjectBinData.Length > 0)
{
File.WriteAllBytes("FullObjectBinData.bin", fullObjectBinData);
Console.WriteLine("Saved FullObjectBin data to file.");
}
// Create another workbook to demonstrate reading the OLE object
Workbook workbook2 = new Workbook();
Worksheet worksheet2 = workbook2.Worksheets[0];
// Add the OLE object from the FullObjectBin data
if (fullObjectBinData != null)
{
int newOleObjectIndex = worksheet2.OleObjects.Add(10, 10, 200, 200, fullObjectBinData, "docx");
Console.WriteLine("Added new OLE object using FullObjectBin data.");
}
// Save the workbooks
workbook.Save("OleObjectWithFullObjectBin.xlsx");
workbook2.Save("OleObjectFromFullObjectBin.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
