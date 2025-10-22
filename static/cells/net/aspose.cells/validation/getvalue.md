##Validation.GetValue
Validation method. Get the value of validation on the specific cell
## Validation.GetValue method
Get the value of validation on the specific cell.
```csharp
public object GetValue(int row, int column, bool isValue1)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
| isValue1 | Boolean | Indicates whether getting the first value. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationMethodGetValueWithInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and validation
worksheet.Cells["A1"].PutValue("Select Item:");
worksheet.Cells["B1"].PutValue("Item 1");
worksheet.Cells["B2"].PutValue("Item 2");
// Create validation for cell B1
Validation validation = worksheet.Cells["B1"].GetValidation();
validation.Type = ValidationType.List;
validation.Formula1 = "A1:B2";
// Get value using GetValue method with row, column and convert numeric to date parameters
object value = validation.GetValue(0, 1, false);
// Output the result
Console.WriteLine("Validation value: " + value.ToString());
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
