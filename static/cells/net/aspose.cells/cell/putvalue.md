##Cell.PutValue
Cell method. Puts a boolean value into the cell
## PutValue(bool) {#putvalue}
Puts a boolean value into the cell.
```csharp
public void PutValue(bool boolValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| boolValue | Boolean |  |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodPutValueWithBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Put a boolean value in cell B3 (row 2, column 2)
cells[2, 2].PutValue(true);
// Verify the value was set correctly
Console.WriteLine("Cell B3 value: " + cells[2, 2].Value);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## PutValue(int) {#putvalue_2}
Puts an integer value into the cell.
```csharp
public void PutValue(int intValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| intValue | Int32 | Input value |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodPutValueWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Using PutValue with Int32 parameters
cells[0, 0].PutValue(10);
cells[1, 0].PutValue(20);
cells[2, 0].PutValue(30);
// Calculate sum of the values
cells[3, 0].Formula = "=SUM(A1:A3)";
workbook.CalculateFormula();
Console.WriteLine("Sum of values: " + cells[3, 0].IntValue);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## PutValue(double) {#putvalue_1}
Puts a double value into the cell.
```csharp
public void PutValue(double doubleValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| doubleValue | Double | Input value |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodPutValueWithDoubleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Put double values using PutValue method
cells[0, 0].PutValue("Item");
cells[0, 1].PutValue("Price");
cells[1, 0].PutValue("Apple");
cells[1, 1].PutValue(0.69);
cells[2, 0].PutValue("Banana");
cells[2, 1].PutValue(0.49);
cells[3, 0].PutValue("Orange");
cells[3, 1].PutValue(0.29);
// Save the workbook
workbook.Save("PutValueWithDoubleDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## PutValue(string, bool, bool) {#putvalue_7}
Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.
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
public class CellMethodPutValueWithStringBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Get cell B3
Cell cell = worksheet.Cells["B3"];
// Set data validation for age (must be positive number)
Validation validation = cell.GetValidation();
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.GreaterThan;
validation.Formula1 = "0";
// Put value with conversion and validation check
cell.PutValue("-60", true, false);
// Calculate formulas (though not needed in this simple case)
workbook.CalculateFormula();
// Check if value is valid
bool isValid = cell.GetValidationValue();
Console.WriteLine("Is value valid? " + isValid);
// Save workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## PutValue(string, bool) {#putvalue_6}
Puts a string value into the cell and converts the value to other data type if appropriate.
```csharp
public void PutValue(string stringValue, bool isConverted)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
| isConverted | Boolean | True: converted to other data type if appropriate. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodPutValueWithStringBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Demonstrate PutValue with string and boolean parameters
cells["B2"].PutValue("123", true);  // String value with conversion flag
cells["C2"].PutValue("456", false); // String value without conversion
// Verify the values
Console.WriteLine("B2 value (converted): " + cells["B2"].Value); // Should show 123 as number
Console.WriteLine("C2 value (raw): " + cells["C2"].Value);       // Should show "456" as string
workbook.Save("PutValueDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## PutValue(string) {#putvalue_5}
Puts a string value into the cell.
```csharp
public void PutValue(string stringValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | String | Input value |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodPutValueWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Using PutValue with string parameters
cells[0, 0].PutValue("Product");
cells[0, 1].PutValue("Category");
cells[0, 2].PutValue("Price");
cells[1, 0].PutValue("Laptop");
cells[1, 1].PutValue("Electronics");
cells[1, 2].PutValue(999.99);
cells[2, 0].PutValue("Desk Chair");
cells[2, 1].PutValue("Furniture");
cells[2, 2].PutValue(199.50);
// Save the workbook
workbook.Save("PutValueStringDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## PutValue(DateTime) {#putvalue_3}
Puts a DateTime value into the cell.
```csharp
public void PutValue(DateTime dateTime)
```
| Parameter | Type | Description |
| --- | --- | --- |
| dateTime | DateTime | Input value |
### Remarks
Setting a DateTime value for a cell dose not means the cell will be formatted as date time automatically. DateTime value was maintained as numeric value in the data model of both ms excel and Aspose.Cells. Whether the numeric value will be taken as the numeric value itself or date time depends on the number format applied on this cell. If this cell has not been formatted as date time, it will be displayed as a numeric value even though what you input is DateTime.
### Examples
This example shows how to set DateTime value to a cell and make it be displayed as date time.
```csharp
[C#]
Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;
//Put date time into a cell
Cell cell = cells[0, 0];
cell.PutValue(new DateTime(2023, 5, 15));
Style style = cell.GetStyle(false);
style.Number = 14;
cell.SetStyle(style);
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## PutValue(object) {#putvalue_4}
Puts an object value into the cell.
```csharp
public void PutValue(object objectValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| objectValue | Object | input value |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodPutValueWithObjectDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// PutValue with DateTime object
DateTime dt = new DateTime(2008, 2, 2);
cells[0, 0].PutValue((object)dt);
// PutValue with string object
cells[1, 0].PutValue((object)"Hello World");
// PutValue with numeric object
cells[2, 0].PutValue((object)123.45);
// Save the workbook
workbook.Save("PutValueWithObjectDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
