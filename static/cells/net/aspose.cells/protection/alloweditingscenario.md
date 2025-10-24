##Protection.AllowEditingScenario
Protection property. Represents if the user is allowed to edit scenarios on a protected worksheet
## Protection.AllowEditingScenario property
Represents if the user is allowed to edit scenarios on a protected worksheet.
```csharp
public bool AllowEditingScenario { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowEditingScenarioDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A2"].PutValue(100);
worksheet.Cells["A3"].PutValue(200);
// Access worksheet protection settings
Protection protection = worksheet.Protection;
// Set protection properties with AllowEditingScenario enabled
protection.AllowEditingScenario = true;
protection.AllowFormattingCell = true;  // Corrected property name
protection.Password = "password123";
// Protect the worksheet
worksheet.Protect(ProtectionType.All);
// Save the workbook
workbook.Save("ProtectionWithScenarioEditing.xlsx");
Console.WriteLine("Worksheet protected with AllowEditingScenario enabled.");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
