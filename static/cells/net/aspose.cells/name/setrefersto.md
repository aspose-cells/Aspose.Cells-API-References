##Name.SetRefersTo
Name method. Set the reference of this Name
## Name.SetRefersTo method
Set the reference of this Name.
```csharp
public void SetRefersTo(string refersTo, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| refersTo | String | The reference. |
| isR1C1 | Boolean | Whether the reference is R1C1 format. |
| isLocal | Boolean | Whether the reference is locale formatted. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class NameMethodSetRefersToWithStringBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Create a named range
int index = workbook.Worksheets.Names.Add("MyNamedRange");
Name namedRange = workbook.Worksheets.Names[index];
try
{
// Call SetRefersTo with parameters (String, Boolean, Boolean)
namedRange.SetRefersTo("=Sheet1!$A$1:$A$3", false, false);
// Display the result
Console.WriteLine($"Named range 'MyNamedRange' now refers to: {namedRange.RefersTo}");
// Verify by using the named range in a formula
worksheet.Cells["B1"].Formula = "=SUM(MyNamedRange)";
workbook.CalculateFormula();
Console.WriteLine($"Result of SUM(MyNamedRange): {worksheet.Cells["B1"].Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetRefersTo method: {ex.Message}");
}
// Save the workbook
workbook.Save("NameMethodSetRefersToWithStringBooleanBooleanDemo.xlsx");
}
}
}
```
### See Also
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
