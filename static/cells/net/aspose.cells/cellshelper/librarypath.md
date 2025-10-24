##CellsHelper.LibraryPath
CellsHelper property. Gets or sets the library path which is referred to by some external formula references
## CellsHelper.LibraryPath property
Gets or sets the library path which is referred to by some external formula references.
```csharp
public static string LibraryPath { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsHelperPropertyLibraryPathDemo
{
public static void Run()
{
// Set the LibraryPath property
CellsHelper.LibraryPath = "C:\\MyLibraries\\AsposeCells";
// Demonstrate getting and using the LibraryPath
Console.WriteLine("Current Library Path: " + CellsHelper.LibraryPath);
// Example of using the path in a file operation
string filePath = System.IO.Path.Combine(CellsHelper.LibraryPath, "test.xlsx");
Console.WriteLine("Would load file from: " + filePath);
}
}
}
```
### See Also
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
