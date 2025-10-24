##ProtectedRange.GetAreas
ProtectedRange method. Gets all referred areas
## ProtectedRange.GetAreas method
Gets all referred areas.
```csharp
public CellArea[] GetAreas()
```
### Return Value
Returns all referred areas.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectedRangeMethodGetAreasDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Get the protected ranges collection
ProtectedRangeCollection protectedRanges = worksheet.AllowEditRanges;
// Add a protected range
int index = protectedRanges.Add("TestRange", 0, 0, 10, 10);
ProtectedRange protectedRange = protectedRanges[index];
// Get areas of the protected range
CellArea[] areas = protectedRange.GetAreas();
// Output the number of areas (should be 1 for this simple range)
Console.WriteLine("Number of areas in protected range: " + areas.Length);
// Save the workbook
workbook.Save("ProtectedRangeExample.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
