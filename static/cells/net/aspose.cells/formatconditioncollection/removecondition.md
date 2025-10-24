##FormatConditionCollection.RemoveCondition
FormatConditionCollection method. Removes the formatting condition by index
## FormatConditionCollection.RemoveCondition method
Removes the formatting condition by index.
```csharp
public void RemoveCondition(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index of the formatting condition to be removed. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FormatConditionCollectionMethodRemoveConditionWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Get the format conditions collection
FormatConditionCollection formatConditions = worksheet.ConditionalFormattings[0];
// Add some sample conditions
int index1 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "10", "100");
int index2 = formatConditions.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "50", "");
try
{
// Display initial count
Console.WriteLine($"Initial conditions count: {formatConditions.Count}");
// Remove the first condition
formatConditions.RemoveCondition(index1);
// Display updated count
Console.WriteLine($"Conditions count after removal: {formatConditions.Count}");
// Save the workbook
workbook.Save("RemoveConditionDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error calling RemoveCondition: {ex.Message}");
}
}
}
}
```
### See Also
* class [FormatConditionCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
