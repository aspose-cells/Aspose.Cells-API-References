##Enum ConsolidationFunction
Aspose.Cells.ConsolidationFunction enum. Represents consolidation function
## ConsolidationFunction enumeration
Represents consolidation function.
```csharp
public enum ConsolidationFunction
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Sum | `0` | Represents Sum function. |
| Count | `1` | Represents Count function. |
| Average | `2` | Represents Average function. |
| Max | `3` | Represents Max function. |
| Min | `4` | Represents Min function. |
| Product | `5` | Represents Product function. |
| CountNums | `6` | Represents Count Nums function. |
| StdDev | `7` | Represents StdDev function. |
| StdDevp | `8` | Represents StdDevp function. |
| Var | `9` | Represents Var function. |
| Varp | `10` | Represents Varp function. |
| DistinctCount | `11` | Represents Distinct Count function. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ConsolidationFunctionDemo
{
public static void ConsolidationFunctionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["A4"].PutValue("C");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["B4"].PutValue(30);
// Define the cell area for subtotal
CellArea cellArea = new CellArea
{
StartRow = 1,
StartColumn = 0,
EndRow = 3,
EndColumn = 1
};
// Apply subtotal with Sum function
worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Sum, new int[] { 1 });
// Apply subtotal with Average function
worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Average, new int[] { 1 });
// Apply subtotal with Max function
worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Max, new int[] { 1 });
// Apply subtotal with Min function
worksheet.Cells.Subtotal(cellArea, 0, ConsolidationFunction.Min, new int[] { 1 });
// Save the workbook
workbook.Save("ConsolidationFunctionExample.xlsx");
workbook.Save("ConsolidationFunctionExample.pdf");
// Output the results
Console.WriteLine("Workbook saved with subtotals applied.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
