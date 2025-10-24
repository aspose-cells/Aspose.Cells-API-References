##Worksheet.AdvancedFilter
Worksheet method. Filters data using complex criteria
## Worksheet.AdvancedFilter method
Filters data using complex criteria.
```csharp
public void AdvancedFilter(bool isFilter, string listRange, string criteriaRange, string copyTo,
bool uniqueRecordOnly)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isFilter | Boolean | Indicates whether filtering the list in place. |
| listRange | String | The list range. |
| criteriaRange | String | The criteria range. |
| copyTo | String | The range where copying data to. |
| uniqueRecordOnly | Boolean | Only displaying or copying unique rows. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAdvancedFilterWithBooleanStringStringStringBooleDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for filtering
// Headers
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Category");
worksheet.Cells["C1"].PutValue("Price");
// Criteria
worksheet.Cells["A2"].PutValue("Product");
worksheet.Cells["B2"].PutValue("Category");
worksheet.Cells["C2"].PutValue("Fruits");
// Data
worksheet.Cells["A4"].PutValue("Apple");
worksheet.Cells["B4"].PutValue("Fruits");
worksheet.Cells["C4"].PutValue(2.5);
worksheet.Cells["A5"].PutValue("Carrot");
worksheet.Cells["B5"].PutValue("Vegetables");
worksheet.Cells["C5"].PutValue(1.2);
worksheet.Cells["A6"].PutValue("Banana");
worksheet.Cells["B6"].PutValue("Fruits");
worksheet.Cells["C6"].PutValue(1.8);
// Apply advanced filter (filter in place, unique records only)
worksheet.AdvancedFilter(false, "A4:C6", "A1:C2", null, true);
// Save the workbook
workbook.Save("AdvancedFilterDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
