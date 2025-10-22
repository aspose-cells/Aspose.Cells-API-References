##PasteOptions.OperationType
PasteOptions property. Gets and sets the operation type when pasting range
## PasteOptions.OperationType property
Gets and sets the operation type when pasting range.
```csharp
public PasteOperationType OperationType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PasteOptionsPropertyOperationTypeDemo
{
public static void Run()
{
// Create source workbook with sample data
Workbook wbOrigin = new Workbook();
Worksheet sourceSheet = wbOrigin.Worksheets[0];
sourceSheet.Cells["A1"].PutValue("Source Data");
sourceSheet.Cells["B2"].PutValue(100);
// Create destination workbook
Workbook wbDestination = new Workbook();
Worksheet destSheet = wbDestination.Worksheets[0];
destSheet.Cells["A1"].PutValue("Destination Data");
destSheet.Cells["B2"].PutValue(200); // Will be modified by paste operation
// Create ranges for copy/paste
var rangeOrigin = sourceSheet.Cells.CreateRange("A1:B3");
var rangeDestination = destSheet.Cells.CreateRange("A1:B3");
// Create paste options with OperationType demonstration
var options = new PasteOptions
{
PasteType = PasteType.All,
OperationType = PasteOperationType.Add // Values will be added (100 + 200 = 300)
};
// Perform the copy/paste operation
rangeDestination.Copy(rangeOrigin, options);
// Verify the result
Console.WriteLine("B2 value after paste with Add operation: " + destSheet.Cells["B2"].IntValue);
// Save the result
wbDestination.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* enum [PasteOperationType](../../pasteoperationtype/)
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
