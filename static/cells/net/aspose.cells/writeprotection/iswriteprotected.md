##WriteProtection.IsWriteProtected
WriteProtection property. Indicates whether this workbook is write protected
## WriteProtection.IsWriteProtected property
Indicates whether this workbook is write protected.
```csharp
public bool IsWriteProtected { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WriteProtectionPropertyIsWriteProtectedDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Enable write protection with password
workbook.Settings.WriteProtection.Password = "1234";
// Check if workbook is write protected
Console.WriteLine("Is workbook write protected? " +
workbook.Settings.WriteProtection.IsWriteProtected);
// Validate the password
Console.WriteLine("Is password valid? " +
workbook.Settings.WriteProtection.ValidatePassword("1234"));
// Save the workbook
workbook.Save("WriteProtectedWorkbook.xlsx");
// Load the saved workbook to verify protection
Workbook loadedWorkbook = new Workbook("WriteProtectedWorkbook.xlsx");
// Check protection status again
Console.WriteLine("Is loaded workbook write protected? " +
loadedWorkbook.Settings.WriteProtection.IsWriteProtected);
}
}
}
```
### See Also
* class [WriteProtection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
