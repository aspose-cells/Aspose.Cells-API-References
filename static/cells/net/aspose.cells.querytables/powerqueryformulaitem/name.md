##PowerQueryFormulaItem.Name
PowerQueryFormulaItem property. Gets the name of the item
## PowerQueryFormulaItem.Name property
Gets the name of the item.
```csharp
public string Name { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PowerQueryFormulaItemPropertyNameDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample Power Query data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(1200);
// Save to trigger Power Query creation
string sourcePath = "pq_source.xlsx";
workbook.Save(sourcePath);
// Reopen to access Power Query formulas
workbook = new Workbook(sourcePath);
Aspose.Cells.QueryTables.DataMashup mashupData = workbook.DataMashup;
// Process Power Query formulas
foreach (Aspose.Cells.QueryTables.PowerQueryFormula formula in mashupData.PowerQueryFormulas)
{
Console.WriteLine("Formula Name: " + formula.Name);
foreach (Aspose.Cells.QueryTables.PowerQueryFormulaItem item in formula.PowerQueryFormulaItems)
{
Console.WriteLine("  Item Name: " + item.Name);
// Demonstrate Name property usage
if (item.Name == "Source")
{
Console.WriteLine("Original Value: " + item.Value);
item.Value = "ModifiedSource";
Console.WriteLine("Modified Value: " + item.Value);
}
}
}
// Save modified workbook
workbook.Save("pq_modified.xlsx");
}
}
}
```
### See Also
* class [PowerQueryFormulaItem](../)
* namespace [Aspose.Cells.QueryTables](../../../aspose.cells.querytables/)
* assembly [Aspose.Cells](../../../)
