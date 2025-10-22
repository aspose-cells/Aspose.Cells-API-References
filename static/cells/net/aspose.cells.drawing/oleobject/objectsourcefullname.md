##OleObject.ObjectSourceFullName
OleObject property. Returns the source full name of the source file for the linked OLE object
## OleObject.ObjectSourceFullName property
Returns the source full name of the source file for the linked OLE object.
```csharp
public string ObjectSourceFullName { get; set; }
```
### Remarks
Only supports setting the source full name when the file type is OleFileType.Unknown. Such as wav file ,avi file..etc..
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OleObjectPropertyObjectSourceFullNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an OLE object (using file data as byte array)
byte[] fileData = System.IO.File.ReadAllBytes("test.docx");
int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, fileData);
Aspose.Cells.Drawing.OleObject oleObject = worksheet.OleObjects[oleObjectIndex];
// Set and get ObjectSourceFullName
oleObject.ObjectSourceFullName = "C:\\Temp\\source.docx";
Console.WriteLine("OLE Object Source Full Name: " + oleObject.ObjectSourceFullName);
// Save the workbook
workbook.Save("OleObjectDemo.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
