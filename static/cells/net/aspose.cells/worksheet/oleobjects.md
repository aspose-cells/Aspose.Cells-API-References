##Worksheet.OleObjects
Worksheet property. Represents a collection of OleObject in a worksheet
## Worksheet.OleObjects property
Represents a collection of [`OleObject`](../../../aspose.cells.drawing/oleobject/) in a worksheet.
```csharp
public OleObjectCollection OleObjects { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class WorksheetPropertyOleObjectsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an OleObject to the worksheet
int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, File.ReadAllBytes(@"C:\temp\example.xlsx"));
OleObject ole = worksheet.OleObjects[oleObjectIndex];
// Modify OleObject properties
ole.ObjectSourceFullName = @"C:\temp\modified.xlsx";
ole.FileFormatType = FileFormatType.Xlsx;
// Save the workbook
workbook.Save(@"C:\temp\output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [OleObjectCollection](../../../aspose.cells.drawing/oleobjectcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
