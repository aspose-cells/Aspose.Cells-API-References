##Protection.AllowEditingObject
Protection property. Represents if the user is allowed to manipulate drawing objects on a protected worksheet
## Protection.AllowEditingObject property
Represents if the user is allowed to manipulate drawing objects on a protected worksheet.
```csharp
public bool AllowEditingObject { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowEditingObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set protection settings with AllowEditingObject enabled
Protection protection = worksheet.Protection;
protection.AllowEditingObject = true;
protection.AllowEditingContent = false; // Contrast with AllowEditingObject
worksheet.Protect(ProtectionType.All);
// Check protection flags
Console.WriteLine("Protection Settings:");
Console.WriteLine($"AllowEditingObject: {protection.AllowEditingObject}");
Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");
// Create a text box (object) to test editing
worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
// Save the workbook
workbook.Save("ProtectionDemo.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
