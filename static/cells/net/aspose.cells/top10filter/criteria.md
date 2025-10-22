##Top10Filter.Criteria
Top10Filter property.
## Top10Filter.Criteria property
```csharp
public object Criteria { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class Top10FilterPropertyCriteriaDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 20; i++)
{
worksheet.Cells[i, 0].PutValue(20 - i);
}
worksheet.AutoFilter.Range = "A1:A20";
worksheet.AutoFilter.FilterTop10(0, true, false, 5);
// Fix: Access Filter property and cast to Top10Filter
Top10Filter filter = (Top10Filter)worksheet.AutoFilter.FilterColumns[0].Filter;
Console.WriteLine("Current Criteria value: " + filter.Criteria);
filter.Criteria = 14;
worksheet.AutoFilter.Refresh();
workbook.Save("Top10FilterCriteriaDemo.xlsx");
}
}
}
```
### See Also
* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
