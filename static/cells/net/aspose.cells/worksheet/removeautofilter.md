##Worksheet.RemoveAutoFilter
Worksheet method. Removes the auto filter of the worksheet
## Worksheet.RemoveAutoFilter method
Removes the auto filter of the worksheet.
```csharp
public void RemoveAutoFilter()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodRemoveAutoFilterDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["A3"].PutValue("Data2");
// Apply auto filter
worksheet.AutoFilter.Range = "A1:A3";
Console.WriteLine("AutoFilter applied: " + worksheet.HasAutofilter);
// Remove auto filter
worksheet.RemoveAutoFilter();
Console.WriteLine("AutoFilter after removal: " + worksheet.HasAutofilter);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
