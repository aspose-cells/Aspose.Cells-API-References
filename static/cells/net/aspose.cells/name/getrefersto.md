##Name.GetRefersTo
Name method. Get the reference of this Name
## GetRefersTo(bool, bool) {#getrefersto}
Get the reference of this Name.
```csharp
public string GetRefersTo(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the reference needs to be formatted by locale. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class NameMethodGetRefersToWithBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
// Create a named range
int index = workbook.Worksheets.Names.Add("MyNamedRange");
Name namedRange = workbook.Worksheets.Names[index];
namedRange.RefersTo = "=Sheet1!$A$1:$A$3";
try
{
// Call GetRefersTo with R1C1 format and local scope
string refersToR1C1Local = namedRange.GetRefersTo(true, true);
Console.WriteLine("R1C1 format with local scope: " + refersToR1C1Local);
// Call GetRefersTo with A1 format and global scope
string refersToA1Global = namedRange.GetRefersTo(false, false);
Console.WriteLine("A1 format with global scope: " + refersToA1Global);
// Show the named range details
Console.WriteLine("Named range text: " + namedRange.Text);
Console.WriteLine("Full text: " + namedRange.FullText);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
}
// Save the workbook
workbook.Save("NameMethodGetRefersToDemo.xlsx");
}
}
}
```
### See Also
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetRefersTo(bool, bool, int, int) {#getrefersto_1}
Get the reference of this Name based on specified cell.
```csharp
public string GetRefersTo(bool isR1C1, bool isLocal, int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the reference needs to be formatted by locale. |
| row | Int32 | The row index of the cell. |
| column | Int32 | The column index of the cell. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo
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
namedRange.RefersTo = "=Sheet1!$A$1:$A$3";
try
{
// Call GetRefersTo with specific parameters (isR1C1, isLocal, row, column)
string refersTo = namedRange.GetRefersTo(false, false, 0, 0);
Console.WriteLine("Named range refers to: " + refersTo);
Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean, Int32, Int32)");
// Modify the named range based on the result
if (!string.IsNullOrEmpty(refersTo))
{
worksheet.Cells["B1"].PutValue("Named Range Refers To:");
worksheet.Cells["B2"].PutValue(refersTo);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetRefersTo method: {ex.Message}");
}
// Save the workbook
workbook.Save("NameMethodGetRefersToWithBooleanBooleanInt32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [Name](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
