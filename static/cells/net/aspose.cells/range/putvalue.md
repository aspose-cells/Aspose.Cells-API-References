##Range.PutValue
Range method. Puts a value into the range if appropriate the value will be converted to other data type and cells number format will be reset
## Range.PutValue method
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
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RangeMethodPutValueWithStringBooleanBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
Aspose.Cells.Range range = cells.CreateRange("A1:B10");
range.PutValue("123", true, false);
Console.WriteLine("Value at A5: " + cells["A5"].DoubleValue);
}
}
}
```
### See Also
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
