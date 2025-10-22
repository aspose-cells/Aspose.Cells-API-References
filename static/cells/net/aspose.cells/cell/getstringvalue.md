##Cell.GetStringValue
Cell method. Gets the string value by specific formatted strategy
## Cell.GetStringValue method
Gets the string value by specific formatted strategy.
```csharp
public string GetStringValue(CellValueFormatStrategy formatStrategy)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formatStrategy | CellValueFormatStrategy | The formatted strategy. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetStringValueWithCellValueFormatStrategyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set different types of data in cells
cells["A1"].PutValue(123.45); // Numeric value
cells["A2"].PutValue(DateTime.Now); // DateTime value
cells["A3"].PutValue(true); // Boolean value
cells["A4"].PutValue("Sample Text"); // String value
// Demonstrate GetStringValue with different format strategies
Console.WriteLine("None: " + cells["A1"].GetStringValue(CellValueFormatStrategy.None));
Console.WriteLine("CellStyle: " + cells["A1"].GetStringValue(CellValueFormatStrategy.CellStyle));
Console.WriteLine("DisplayString: " + cells["A1"].GetStringValue(CellValueFormatStrategy.DisplayString));
Console.WriteLine("DateTime None: " + cells["A2"].GetStringValue(CellValueFormatStrategy.None));
Console.WriteLine("DateTime CellStyle: " + cells["A2"].GetStringValue(CellValueFormatStrategy.CellStyle));
}
}
}
```
### See Also
* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
