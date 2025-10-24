##OleObject.Label
OleObject property. Gets and sets the display label of the linked ole object
## OleObject.Label property
Gets and sets the display label of the linked ole object.
```csharp
public string Label { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class OleObjectPropertyLabelDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an OLE object with a label
int oleIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]);
OleObject oleObject = worksheet.OleObjects[oleIndex];
oleObject.Label = "label_nameです";
// Save and reload the workbook
string outputPath = "output.xlsx";
workbook.Save(outputPath);
// Verify the label property
Workbook loadedWorkbook = new Workbook(outputPath);
OleObject loadedOleObject = loadedWorkbook.Worksheets[0].OleObjects[0];
Console.WriteLine("OLE Object Label: " + loadedOleObject.Label);
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
