##Protection.AllowFiltering
Protection property. Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected
## Protection.AllowFiltering property
Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected.
```csharp
public bool AllowFiltering { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowFilteringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Enable worksheet protection
worksheet.Protect(ProtectionType.All);
// Set AllowFiltering property to true
worksheet.Protection.AllowFiltering = true;
// Save the workbook
workbook.Save("output.xlsx");
// Verify the property was saved correctly
Workbook loadedWorkbook = new Workbook("output.xlsx");
Console.WriteLine("AllowFiltering: " +
loadedWorkbook.Worksheets[0].Protection.AllowFiltering);
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
