##ProtectedRange.Name
ProtectedRange property. Gets the Range title. This is used as a descriptor not as a named range definition
## ProtectedRange.Name property
Gets the Range title. This is used as a descriptor, not as a named range definition.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ProtectedRangePropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create protected range collection
ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
// Add a protected range with name "MyRange"
int index = allowRanges.Add("MyRange", 0, 0, 2, 2);
ProtectedRange protectedRange = allowRanges[index];
protectedRange.Password = "123";
// Access and display the Name property
Console.WriteLine("Protected range name: " + protectedRange.Name);
Console.WriteLine("Cell area: {0},{1} to {2},{3}",
protectedRange.CellArea.StartRow,
protectedRange.CellArea.StartColumn,
protectedRange.CellArea.EndRow,
protectedRange.CellArea.EndColumn);
// Add another named range
index = allowRanges.Add("SecondRange", 3, 3, 5, 5);
ProtectedRange secondRange = allowRanges[index];
Console.WriteLine("Second protected range name: " + secondRange.Name);
// Save the workbook
workbook.Save("ProtectedRangeDemo.xlsx");
}
}
}
```
### See Also
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
