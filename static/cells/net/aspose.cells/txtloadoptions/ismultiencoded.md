##TxtLoadOptions.IsMultiEncoded
TxtLoadOptions property. True means that the file contains several encoding
## TxtLoadOptions.IsMultiEncoded property
True means that the file contains several encoding.
```csharp
public bool IsMultiEncoded { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtLoadOptionsPropertyIsMultiEncodedDemo
{
public static void Run()
{
// Create text load options
TxtLoadOptions options = new TxtLoadOptions();
// Set IsMultiEncoded to true to handle multiple encodings
options.IsMultiEncoded = true;
// Load workbook with the options
Workbook workbook = new Workbook("example.csv", options);
// Display sample values from the loaded file
Console.WriteLine("A2 Cell Value: " + workbook.Worksheets[0].Cells["A2"].StringValue);
Console.WriteLine("A3 Cell Value: " + workbook.Worksheets[0].Cells["A3"].StringValue);
}
}
}
```
### See Also
* class [TxtLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
