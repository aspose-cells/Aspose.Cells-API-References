##Row.Equals
Row method. Checks whether this object refers to the same row with another
## Equals(object) {#equals_1}
Checks whether this object refers to the same row with another.
```csharp
public override bool Equals(object obj)
```
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | another object |
### Return Value
true if two objects refers to the same row.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class RowMethodEqualsWithObjectDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two rows to compare
Row row1 = worksheet.Cells.Rows[0];
Row row2 = worksheet.Cells.Rows[1];
// Set some properties to make rows different
row1.Height = 20;
row2.Height = 25;
try
{
// Call the Equals method with Object parameter
bool result1 = row1.Equals((object)row2);
Console.WriteLine($"Comparing row1 with row2: {result1}");
// Compare row1 with itself
bool result2 = row1.Equals((object)row1);
Console.WriteLine($"Comparing row1 with itself: {result2}");
// Compare with null
bool result3 = row1.Equals((object)null);
Console.WriteLine($"Comparing row1 with null: {result3}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
workbook.Save("RowMethodEqualsWithObjectDemo.xlsx");
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Equals(Row) {#equals}
Checks whether this object refers to the same row with another row object.
```csharp
public bool Equals(Row row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Row | another row object |
### Return Value
true if two row objects refers to the same row.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class RowMethodEqualsWithRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create two rows to compare
Row row1 = worksheet.Cells.Rows[0];
Row row2 = worksheet.Cells.Rows[1];
// Set some properties to make rows different
row1.Height = 20;
row2.Height = 25;
row1.IsHidden = false;
row2.IsHidden = true;
try
{
// Call the Equals method to compare the rows
bool areEqual = row1.Equals(row2);
// Display the result
Console.WriteLine($"Are rows equal? {areEqual}");
// Create another row with same properties as row1
Row row3 = worksheet.Cells.Rows[2];
row3.Height = row1.Height;
row3.IsHidden = row1.IsHidden;
// Compare row1 with row3 (should be equal)
bool areEqual2 = row1.Equals(row3);
Console.WriteLine($"Are rows equal after matching properties? {areEqual2}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing Equals method: {ex.Message}");
}
// Save the workbook
workbook.Save("RowEqualsDemo.xlsx");
}
}
}
```
### See Also
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
