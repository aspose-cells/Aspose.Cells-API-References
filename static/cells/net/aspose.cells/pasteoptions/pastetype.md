##PasteOptions.PasteType
PasteOptions property. The paste special type
## PasteOptions.PasteType property
The paste special type.
```csharp
public PasteType PasteType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PasteOptionsPropertyPasteTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set source value
worksheet.Cells["A1"].PutValue("SourceValue");
// Create ranges with fully qualified type names
Aspose.Cells.Range sourceRange = worksheet.Cells.CreateRange("A1");
Aspose.Cells.Range targetRange = worksheet.Cells.CreateRange("B1:D3");
// Copy with PasteType.All
targetRange.Copy(sourceRange, new PasteOptions() { PasteType = PasteType.All });
// Output results
Console.WriteLine("A1: " + worksheet.Cells["A1"].StringValue);
Console.WriteLine("B1: " + worksheet.Cells["B1"].StringValue);
Console.WriteLine("C2: " + worksheet.Cells["C2"].StringValue);
Console.WriteLine("D3: " + worksheet.Cells["D3"].StringValue);
}
}
}
```
### See Also
* enum [PasteType](../../pastetype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
