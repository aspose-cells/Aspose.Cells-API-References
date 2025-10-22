##Protection.AllowSelectingUnlockedCell
Protection property. Represents if the user is allowed to select unlocked cells on a protected worksheet
## Protection.AllowSelectingUnlockedCell property
Represents if the user is allowed to select unlocked cells on a protected worksheet.
```csharp
public bool AllowSelectingUnlockedCell { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowSelectingUnlockedCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Protect the worksheet with all protection options
Protection protection = worksheet.Protection;
// Set AllowSelectingUnlockedCell to true
protection.AllowSelectingUnlockedCell = true;
protection.AllowSelectingLockedCell = false;
// Apply protection with password
protection.Password = "password123";
worksheet.Protect(ProtectionType.All);
// Verify the setting
Console.WriteLine("AllowSelectingUnlockedCell: " + protection.AllowSelectingUnlockedCell);
Console.WriteLine("Worksheet is protected: " + worksheet.IsProtected);
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
