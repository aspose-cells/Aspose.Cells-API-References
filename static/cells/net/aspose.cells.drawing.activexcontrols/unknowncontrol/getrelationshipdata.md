##UnknownControl.GetRelationshipData
UnknownControl method. Gets the related data
## UnknownControl.GetRelationshipData method
Gets the related data.
```csharp
public byte[] GetRelationshipData(string relId)
```
| Parameter | Type | Description |
| --- | --- | --- |
| relId | String | The relationship id. |
### Return Value
Returns the related data.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
public class UnknownControlMethodGetRelationshipDataWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Attempt to add unknown ActiveX control
Shape shape;
try
{
shape = worksheet.Shapes.AddActiveXControl(ControlType.Unknown, 0, 0, 0, 0, 100, 100);
}
catch (ArgumentException ex)
{
Console.WriteLine($"Could not create control: {ex.Message}");
return;
}
// Get control as UnknownControl
UnknownControl unknownControl = shape.ActiveXControl as UnknownControl;
if (unknownControl == null)
{
Console.WriteLine("ActiveX control is not UnknownControl type");
return;
}
try
{
// Execute GetRelationshipData with string parameter
string relationshipId = "rId1";
byte[] relationshipData = unknownControl.GetRelationshipData(relationshipId);
Console.WriteLine("GetRelationshipData executed successfully");
Console.WriteLine(relationshipData == null
? "No relationship data found"
: $"Received {relationshipData.Length} bytes of data");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
workbook.Save("UnknownControlGetRelationshipDataDemo.xlsx");
}
}
}
```
### See Also
* class [UnknownControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)
