##Worksheet.Cells
Worksheet property. Gets the Cells collection
## Worksheet.Cells property
Gets the `Cells` collection.
```csharp
public Cells Cells { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyCellsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access cells collection
Cells cells = worksheet.Cells;
// Set values in cells
cells["A1"].PutValue("Item");
cells["B1"].PutValue("Price");
cells["A2"].PutValue("Apple");
cells["B2"].PutValue(2.5);
cells["A3"].PutValue("Orange");
cells["B3"].PutValue(1.8);
// Set formula to calculate total
cells["A4"].PutValue("Total:");
cells["B4"].Formula = "=SUM(B2:B3)";
// Calculate formulas
workbook.CalculateFormula();
// Display cell values
Console.WriteLine("A1: " + cells["A1"].StringValue);
Console.WriteLine("B1: " + cells["B1"].StringValue);
Console.WriteLine("A2: " + cells["A2"].StringValue);
Console.WriteLine("B2: " + cells["B2"].StringValue);
Console.WriteLine("A3: " + cells["A3"].StringValue);
Console.WriteLine("B3: " + cells["B3"].StringValue);
Console.WriteLine("A4: " + cells["A4"].StringValue);
Console.WriteLine("B4: " + cells["B4"].StringValue + " (Formula: " + cells["B4"].Formula + ")");
// Save workbook
workbook.Save("CellsPropertyDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cells](../../cells/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
