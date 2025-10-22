##Protection.Copy
Protection method. Copy protection info
## Protection.Copy method
Copy protection info.
```csharp
public void Copy(Protection source)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | Protection |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ProtectionMethodCopyWithProtectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create source protection settings - use existing protection from worksheet
Protection sourceProtection = worksheet.Protection;
sourceProtection.AllowDeletingColumn = true;
sourceProtection.AllowInsertingRow = false;
sourceProtection.Password = "test123";
sourceProtection.AllowFormattingCell = true;
// Get target protection settings
Protection targetProtection = worksheet.Protection;
try
{
// Call the Copy method with Protection parameter
targetProtection.Copy(sourceProtection);
Console.WriteLine("Protection settings copied successfully.");
Console.WriteLine($"Target protection - AllowDeletingColumn: {targetProtection.AllowDeletingColumn}");
Console.WriteLine($"Target protection - AllowInsertingRow: {targetProtection.AllowInsertingRow}");
Console.WriteLine($"Target protection - Password set: {!string.IsNullOrEmpty(targetProtection.Password)}");
}
catch (Exception ex)
{
Console.WriteLine($"Error copying protection settings: {ex.Message}");
}
// Save the workbook
workbook.Save("ProtectionCopyDemo.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
