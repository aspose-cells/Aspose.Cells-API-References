##CellsHelper.StartupPath
CellsHelper property. Gets or sets the startup path which is referred to by some external formula references
## CellsHelper.StartupPath property
Gets or sets the startup path, which is referred to by some external formula references.
```csharp
public static string StartupPath { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperPropertyStartupPathDemo
{
public static void Run()
{
// Set the startup path
CellsHelper.StartupPath = "C:\\Temp\\AsposeCellsStartup";
// Display the startup path
Console.WriteLine("Startup Path: " + CellsHelper.StartupPath);
// Demonstrate additional CellsHelper properties
CellsHelper.SignificantDigits = 15;
Console.WriteLine("Significant Digits: " + CellsHelper.SignificantDigits);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
