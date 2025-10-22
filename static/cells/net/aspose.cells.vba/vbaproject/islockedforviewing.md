##VbaProject.IslockedForViewing
VbaProject property. Indicates whether this VBA project is locked for viewing
## VbaProject.IslockedForViewing property
Indicates whether this VBA project is locked for viewing.
```csharp
public bool IslockedForViewing { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Vba;
namespace AsposeCellsExamples
{
public class VbaProjectPropertyIslockedForViewingDemo
{
public static void Run()
{
// Create a sample workbook with VBA project
Workbook wb = new Workbook();
// Create a new worksheet to ensure VBA project is created
wb.Worksheets.Add();
// Demonstrate IslockedForViewing property
Console.WriteLine("Initial state:");
Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");
// Protect and lock for viewing
wb.VbaProject.Protect(true, "password123");
Console.WriteLine("After protecting and locking for viewing:");
Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");
// Protect without locking for viewing
wb.VbaProject.Protect(false, "password456");
Console.WriteLine("After protecting without locking for viewing:");
Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}\n");
// Remove protection
wb.VbaProject.Protect(true, "");
Console.WriteLine("After removing protection:");
Console.WriteLine($"IsProtected: {wb.VbaProject.IsProtected}");
Console.WriteLine($"IslockedForViewing: {wb.VbaProject.IslockedForViewing}");
}
}
}
```
### See Also
* class [VbaProject](../)
* namespace [Aspose.Cells.Vba](../../../aspose.cells.vba/)
* assembly [Aspose.Cells](../../../)
