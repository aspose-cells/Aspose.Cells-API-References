##Validation.GetListValue
Validation method. Get the value for list of the validation for the specified cell
## Validation.GetListValue method
Get the value for list of the validation for the specified cell.
```csharp
public object GetListValue(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
### Return Value
The value to produce the list of this validation for the specified cell. If the list references to a range, then the returned value will be a [`ReferredArea`](../../referredarea/) object; Otherwise the returned value may be null, object[], or simple object.
### Remarks
Only for validation whose type is List and has been applied to given cell, otherwise null will be returned.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationMethodGetListValueWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for validation
worksheet.Cells["A1"].PutValue("Apple");
worksheet.Cells["A2"].PutValue("Banana");
worksheet.Cells["A3"].PutValue("Cherry");
worksheet.Cells["A4"].PutValue("Date");
// Create validation for cell B1
Validation validation = worksheet.Cells["B1"].GetValidation();
validation.Type = ValidationType.List;
validation.Formula1 = "A1:A4";
// Test GetListValue with different parameters
Console.WriteLine("List values:");
for (int i = 0; i < 4; i++)
{
object value = validation.GetListValue(i, 0);
Console.WriteLine($"Index {i}: {value}");
}
// Change to comma-separated values
validation.Formula1 = "Red,Green,Blue";
Console.WriteLine("\nComma-separated values:");
for (int i = 0; i < 3; i++)
{
object[] values = (object[])validation.GetListValue(i, 0);
Console.WriteLine($"Index {i}: {string.Join(", ", values)}");
}
// Change to single value
validation.Formula1 = "SingleValue";
Console.WriteLine("\nSingle value:");
object singleValue = validation.GetListValue(0, 0);
Console.WriteLine($"Value: {singleValue}");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
