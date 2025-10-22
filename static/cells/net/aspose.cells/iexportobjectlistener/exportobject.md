##IExportObjectListener.ExportObject
IExportObjectListener method. Export one object
## IExportObjectListener.ExportObject method
Export one object.
```csharp
public object ExportObject(ExportObjectEvent e)
```
| Parameter | Type | Description |
| --- | --- | --- |
| e | ExportObjectEvent | The event triggered when one object needs to be exported. |
### Return Value
The information about the result of exporting object. For exporting objects when export workbook to HTML format, the result is URL string to access the saved Image from the html file which contains this exported object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class IExportObjectListenerMethodExportObjectWithExportObjectEventDemo : IExportObjectListener
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
Picture picture = worksheet.Pictures[pictureIndex];
// Create an instance of the demo class implementing IExportObjectListener
var listener = new IExportObjectListenerMethodExportObjectWithExportObjectEventDemo();
try
{
// In a real scenario, the ExportObjectEvent would be provided by the framework
// For demo purposes, we'll just call the method with null
object result = listener.ExportObject(null);
Console.WriteLine("ExportObject method executed successfully.");
Console.WriteLine($"Returned object type: {result?.GetType().Name ?? "null"}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ExportObject method: {ex.Message}");
}
workbook.Save("ExportObjectDemo.xlsx");
}
public object ExportObject(ExportObjectEvent e)
{
// Custom implementation to handle the export
if (e != null)
{
object source = e.GetSource();
Console.WriteLine($"Exporting object of type: {source?.GetType().Name ?? "null"}");
}
else
{
Console.WriteLine("No export event provided (demo mode)");
}
// Return a modified object or null to use default export behavior
return null;
}
}
}
```
### See Also
* class [ExportObjectEvent](../../exportobjectevent/)
* interface [IExportObjectListener](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
