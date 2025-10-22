##PivotTable.ShowReportFilterPageByIndex
PivotTable method. Show all the report filter pages according to the position index in the PageFields
## PivotTable.ShowReportFilterPageByIndex method
Show all the report filter pages according to the position index in the PageFields
```csharp
public void ShowReportFilterPageByIndex(int posIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| posIndex | Int32 | The position index in the PageFields |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodShowReportFilterPageByIndexWithInt32Demo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("PivotTable.xlsx");
// Access the first worksheet which contains the pivot table
Worksheet worksheet = workbook.Worksheets[0];
// Access the first pivot table
PivotTable pivotTable = worksheet.PivotTables[0];
// Show report filter pages by index (position) of the page field
int pageFieldIndex = 0; // First page field
pivotTable.ShowReportFilterPageByIndex(pageFieldIndex);
// Save the workbook
workbook.Save("PivotTable_ShowReportFilterPageByIndex_Output.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
