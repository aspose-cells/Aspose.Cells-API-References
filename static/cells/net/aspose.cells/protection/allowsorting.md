##Protection.AllowSorting
Protection property. Represents if the sorting option is allowed on a protected worksheet
## Protection.AllowSorting property
Represents if the sorting option is allowed on a protected worksheet.
```csharp
public bool AllowSorting { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowSortingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Enable worksheet protection
worksheet.Protect(ProtectionType.All);
// Set protection properties including AllowSorting
Protection protection = worksheet.Protection;
protection.AllowSorting = true;
protection.AllowFiltering = true;
protection.AllowEditingContent = false;
// Output protection settings
Console.WriteLine("Protection Settings:");
Console.WriteLine($"AllowSorting: {protection.AllowSorting}");
Console.WriteLine($"AllowFiltering: {protection.AllowFiltering}");
Console.WriteLine($"AllowEditingContent: {protection.AllowEditingContent}");
// Demonstrate sorting capability
if (protection.AllowSorting)
{
Console.WriteLine("\nSorting is allowed on this protected worksheet");
}
else
{
Console.WriteLine("\nSorting is not allowed on this protected worksheet");
}
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
