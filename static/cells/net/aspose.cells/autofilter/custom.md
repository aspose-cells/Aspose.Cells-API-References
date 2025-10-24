##AutoFilter.Custom
AutoFilter method. Filters a list with a custom criteria
## Custom(int, FilterOperatorType, object) {#custom}
Filters a list with a custom criteria.
```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| operatorType1 | FilterOperatorType | The filter operator type |
| criteria1 | Object | The custom criteria |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to column A (10 rows + header)
worksheet.Cells["A1"].PutValue("Numbers");
for (int i = 1; i <= 10; i++)
{
worksheet.Cells[i, 0].PutValue(i); // A2-A11: 1-10
}
// Set autofilter range (A1:A11)
worksheet.AutoFilter.SetRange(0, 0, 0);
try
{
// Apply custom filter: Numbers > 5
worksheet.AutoFilter.Custom(0, FilterOperatorType.GreaterThan, 5);
// Refresh filter to apply changes
worksheet.AutoFilter.Refresh();
Console.WriteLine("Custom filter applied: Column 0 values > 5");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Custom method: {ex.Message}");
}
// Save the filtered workbook
workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectDemo.xlsx");
}
}
}
```
### See Also
* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Custom(int, FilterOperatorType, object, bool, FilterOperatorType, object) {#custom_1}
Filters a list with custom criteria.
```csharp
public void Custom(int fieldIndex, FilterOperatorType operatorType1, object criteria1, bool isAnd,
FilterOperatorType operatorType2, object criteria2)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | Int32 | The integer offset of the field on which you want to base the filter (from the left of the list; the leftmost field is field 0). |
| operatorType1 | FilterOperatorType | The filter operator type |
| criteria1 | Object | The custom criteria |
| isAnd | Boolean |  |
| operatorType2 | FilterOperatorType | The filter operator type |
| criteria2 | Object | The custom criteria |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data
worksheet.Cells["A1"].PutValue("Product ID");
worksheet.Cells["A2"].PutValue(85);
worksheet.Cells["A3"].PutValue(42);
worksheet.Cells["A4"].PutValue(65);
worksheet.Cells["A5"].PutValue(95);
worksheet.Cells["A6"].PutValue(30);
worksheet.Cells["A7"].PutValue(75);
// Set auto filter range (A1:A7)
AutoFilter autoFilter = worksheet.AutoFilter;
autoFilter.SetRange(0, 0, 0); // Start row: 0 (A1), strartt column: 0 (A), end Column: 0 (A)
try
{
// Apply custom filter: Greater than or equal to 50 AND Less than or equal to 100
autoFilter.Custom(
0, // Field index (column A)
FilterOperatorType.GreaterOrEqual,
50, // First criteria
true, // AND combination
FilterOperatorType.LessOrEqual,
100 // Second criteria
);
Console.WriteLine("Custom filter applied successfully with parameters: " +
"(Int32, FilterOperatorType, Object, Boolean, FilterOperatorType, Object)");
// Refresh filters and save results
autoFilter.Refresh();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Custom method: {ex.Message}");
}
// Save the filtered workbook
workbook.Save("AutoFilterMethodCustomWithInt32FilterOperatorTypeObjectBDemo.xlsx");
}
}
}
```
### See Also
* enum [FilterOperatorType](../../filteroperatortype/)
* class [AutoFilter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
