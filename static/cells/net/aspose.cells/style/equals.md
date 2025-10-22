##Style.Equals
Style method. Determines whether two Style instances are equal
## Style.Equals method
Determines whether two Style instances are equal.
```csharp
public override bool Equals(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The Style object to compare with the current Style object. |
### Return Value
true if the specified Object is equal to the current Object; otherwise, false.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class StyleMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two styles to compare
Style style1 = workbook.CreateStyle();
style1.Font.Name = "Arial";
style1.Font.Size = 12;
style1.HorizontalAlignment = TextAlignmentType.Center;
Style style2 = workbook.CreateStyle();
style2.Font.Name = "Arial";
style2.Font.Size = 12;
style2.HorizontalAlignment = TextAlignmentType.Center;
try
{
// Call the Equals method to compare the styles
bool areEqual = style1.Equals((object)style2);
// Display the result
Console.WriteLine($"The styles are equal: {areEqual}");
// Apply the styles to demonstrate they are identical
if (areEqual)
{
Cell cell1 = worksheet.Cells["A1"];
cell1.PutValue("Style 1");
cell1.SetStyle(style1);
Cell cell2 = worksheet.Cells["A2"];
cell2.PutValue("Style 2");
cell2.SetStyle(style2);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the result
workbook.Save("StyleEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
