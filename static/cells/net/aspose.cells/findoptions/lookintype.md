##FindOptions.LookInType
FindOptions property. Look in type
## FindOptions.LookInType property
Look in type.
```csharp
public LookInType LookInType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsPropertyLookInTypeDemo
{
public static void Run()
{
// Create a workbook and add sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set values and formulas in cells
worksheet.Cells["A1"].PutValue("SearchValue");
worksheet.Cells["A2"].Formula = "=A1";
worksheet.Cells["B1"].PutValue("OtherValue");
// Create find options to search only in formulas
FindOptions options = new FindOptions
{
LookInType = LookInType.OnlyFormulas,
LookAtType = LookAtType.Contains
};
// Search for the value in formulas
Cell foundCell = worksheet.Cells.Find("SearchValue", null, options);
// Output the result
if (foundCell != null)
{
Console.WriteLine($"Found at: Row {foundCell.Row}, Column {foundCell.Column}");
}
else
{
Console.WriteLine("Value not found in formulas");
}
}
}
}
```
### See Also
* enum [LookInType](../../lookintype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
