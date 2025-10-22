##OleObject.SetNativeSourceFullName
OleObject method. Sets the ole native source full file name with path
## OleObject.SetNativeSourceFullName method
Sets the ole native source full file name with path.
```csharp
public void SetNativeSourceFullName(string sourceFullName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceFullName | String | the ole native source full file name |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class OleObjectMethodSetNativeSourceFullNameWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an OleObject to the worksheet
int oleObjectIndex = worksheet.OleObjects.Add(10, 10, 200, 200, new byte[0]); // Changed to empty byte array
OleObject oleObject = worksheet.OleObjects[oleObjectIndex];
try
{
// Call the SetNativeSourceFullName method with a string parameter
oleObject.SetNativeSourceFullName(@"C:\temp\updated_test.xlsx");
Console.WriteLine("SetNativeSourceFullName method executed successfully with parameter: C:\\temp\\updated_test.xlsx");
// Display the effect by checking the ObjectSourceFullName property
Console.WriteLine($"OleObject's source is now: {oleObject.ObjectSourceFullName}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetNativeSourceFullName method: {ex.Message}");
}
// Save the workbook
workbook.Save("OleObjectMethodSetNativeSourceFullNameDemo.xlsx");
}
}
}
```
### See Also
* class [OleObject](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
