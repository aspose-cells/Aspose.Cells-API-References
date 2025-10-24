##LoadOptions.IgnoreUselessShapes
LoadOptions property. Indicates whether ignoring useless shapes
## LoadOptions.IgnoreUselessShapes property
Indicates whether ignoring useless shapes.
```csharp
public bool IgnoreUselessShapes { get; set; }
```
### Remarks
Only works for xlsx,xlsb, and xlsm files. There are many overlapping identical shapes which are useless in some files, we can ingore them when loading files.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyIgnoreUselessShapesDemo
{
public static void Run()
{
// Create load options and set IgnoreUselessShapes to true
LoadOptions options = new LoadOptions();
options.IgnoreUselessShapes = true;
// Load workbook with the options
Workbook workbook = new Workbook("example.xlsx", options);
// Output the count of shapes in the first worksheet
Console.WriteLine("Shapes count: " + workbook.Worksheets[0].Shapes.Count);
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
