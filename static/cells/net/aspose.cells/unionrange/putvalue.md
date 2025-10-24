##UnionRange.PutValue
UnionRange method. Puts a value into the range if appropriate the value will be converted to other data type and cells number format will be reset
## UnionRange.PutValue method
Puts a value into the range, if appropriate the value will be converted to other data type and cell's number format will be reset.
```csharp
public void PutValue(string stringValue, bool isConverted, bool setStyle)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | Boolean | True: converted to other data type if appropriate. |
| setStyle | Boolean | True: set the number format to cell's style when converting to other data type |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class UnionRangeMethodPutValueWithStringBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a union range covering cells A1 to B2
UnionRange unionRange = worksheet.Cells.CreateRange("A1:B2").UnionRanges(new Aspose.Cells.Range[] { worksheet.Cells.CreateRange("A1:B2") });
try
{
// Call PutValue with parameters: (String, Boolean, Boolean)
unionRange.PutValue("Sample Value", true, true);
Console.WriteLine("PutValue method executed successfully with parameters (String, Boolean, Boolean)");
// Display the range information to show the effect
Console.WriteLine($"Range address: {unionRange.RefersTo}");
Console.WriteLine($"Value set in range: {unionRange.Value}");
// Apply formatting to make the effect visible
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
style.HorizontalAlignment = TextAlignmentType.Center;
unionRange.SetStyle(style);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing PutValue method: {ex.Message}");
}
// Save the result
workbook.Save("UnionRangeMethodPutValueWithStringBooleanBooleanDemo.xlsx");
}
}
}
```
### See Also
* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
