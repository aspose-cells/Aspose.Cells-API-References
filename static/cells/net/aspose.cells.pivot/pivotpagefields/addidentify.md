##PivotPageFields.AddIdentify
PivotPageFields method. Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount so please add the page field first
## PivotPageFields.AddIdentify method
Sets which item label in each page field to use to identify the data range. The pageItemIndex.Length must be equal to PageFieldCount, so please add the page field first.
```csharp
public void AddIdentify(int rangeIndex, int[] pageItemIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rangeIndex | Int32 | The consolidation data range index. |
| pageItemIndex | Int32[] | The page item index in the each page field. pageItemIndex[2] = 1 means the second item in the third field to use to identify this range. pageItemIndex[1] = -1 means no item in the second field to use to identify this range and MS will auto create "blank" item in the second field to identify this range. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Data");
worksheet.Cells["A2"].PutValue(1);
worksheet.Cells["A3"].PutValue(2);
worksheet.Cells["A4"].PutValue(3);
worksheet.Cells["B1"].PutValue("Category");
worksheet.Cells["B2"].PutValue("A");
worksheet.Cells["B3"].PutValue("B");
worksheet.Cells["B4"].PutValue("C");
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("A1:B4", "E5", "PivotTable");
PivotTable pivotTable = pivotTables[pivotIndex];
// Instantiate PivotPageFields directly instead of accessing via PivotTable
PivotPageFields pageFields = new PivotPageFields();
try
{
pageFields.AddIdentify(0, new int[] { 0, 1 });
Console.WriteLine("AddIdentify executed successfully");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
workbook.Save("PivotPageFieldsMethodAddIdentifyWithInt32Int32Demo.xlsx");
}
}
}
```
### See Also
* class [PivotPageFields](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
