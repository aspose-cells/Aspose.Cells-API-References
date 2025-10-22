##CellsHelper.AltStartPath
CellsHelper property. Gets or sets the alternate startup path which is referred to by some external formula references
## CellsHelper.AltStartPath property
Gets or sets the alternate startup path, which is referred to by some external formula references.
```csharp
public static string AltStartPath { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperPropertyAltStartPathDemo
{
public static void Run()
{
// Set the alternate startup path
CellsHelper.AltStartPath = "D:\\Aspose\\Cells";
// Also set other relevant properties for demonstration
CellsHelper.StartupPath = "C:\\Program Files\\Aspose\\Cells";
// Display the paths to demonstrate the property usage
Console.WriteLine("Main Startup Path: " + CellsHelper.StartupPath);
Console.WriteLine("Alternate Startup Path: " + CellsHelper.AltStartPath);
// Example of how these paths might be used
Console.WriteLine("\nWhen resources aren't found in main path, system will check: " + CellsHelper.AltStartPath);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
