##Protection.AllowSelectingLockedCell
Protection property. Represents if the user is allowed to select locked cells on a protected worksheet
## Protection.AllowSelectingLockedCell property
Represents if the user is allowed to select locked cells on a protected worksheet.
```csharp
public bool AllowSelectingLockedCell { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowSelectingLockedCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set protection settings
Protection protection = worksheet.Protection;
// Demonstrate AllowSelectingLockedCell property
protection.AllowSelectingLockedCell = true;
Console.WriteLine("AllowSelectingLockedCell is set to: " + protection.AllowSelectingLockedCell);
// Modify the property and show the change
protection.AllowSelectingLockedCell = false;
Console.WriteLine("AllowSelectingLockedCell is now set to: " + protection.AllowSelectingLockedCell);
// Protect the worksheet with password
protection.Password = "password123";
worksheet.Protect(ProtectionType.All);
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
