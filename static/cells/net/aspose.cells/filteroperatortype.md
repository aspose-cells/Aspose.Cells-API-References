##Enum FilterOperatorType
Aspose.Cells.FilterOperatorType enum. Custom Filter operator type
## FilterOperatorType enumeration
Custom Filter operator type.
```csharp
public enum FilterOperatorType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| LessOrEqual | `0` | Represents LessOrEqual operator. |
| LessThan | `1` | Represents LessThan operator. |
| Equal | `2` | Represents Equal operator. |
| GreaterThan | `3` | Represents GreaterThan operator. |
| NotEqual | `4` | Represents NotEqual operator. |
| GreaterOrEqual | `5` | Represents GreaterOrEqual operator. |
| None | `6` | Represents no comparison. |
| BeginsWith | `7` | Begins with the text. |
| EndsWith | `8` | Ends with the text. |
| Contains | `9` | Contains the text. |
| NotContains | `10` | Not contains the text. |
| NotBeginsWith | `11` | Not begins with the text. |
| NotEndsWith | `12` | Not ends with the text. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassFilterOperatorTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Names");
worksheet.Cells["A2"].PutValue("Bob");
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["A4"].PutValue("Bobby");
worksheet.Cells["A5"].PutValue("Tom");
// Set auto filter range
worksheet.AutoFilter.Range = "A1:A5";
// Apply custom filter to show names beginning with "Bo"
worksheet.AutoFilter.Custom(0, FilterOperatorType.BeginsWith, "Bo");
// Refresh the filter
worksheet.AutoFilter.Refresh();
// Save the workbook
workbook.Save("FilterOperatorTypeDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
