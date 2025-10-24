##ValidationCollection.Item
ValidationCollection property. Gets the Validation element at the specified index
## ValidationCollection indexer
Gets the [`Validation`](../../validation/) element at the specified index.
```csharp
public Validation this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add data validation to cells
ValidationCollection validations = sheet.Validations;
// First validation area
Validation validation1 = validations[validations.Add()];
validation1.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 4, EndColumn = 3 });
// Second validation area
Validation validation2 = validations[validations.Add()];
validation2.AddArea(new CellArea { StartRow = 6, StartColumn = 1, EndRow = 6, EndColumn = 3 });
// Access validation using Item property
Validation firstValidation = validations[0];
Console.WriteLine($"First validation has {firstValidation.Areas.Length} area(s)");
// Verify areas
foreach (CellArea area in firstValidation.Areas)
{
Console.WriteLine($"Area: {area.StartRow},{area.StartColumn} to {area.EndRow},{area.EndColumn}");
}
}
}
}
```
### See Also
* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
