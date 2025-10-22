##Enum LoadDataFilterOptions
Aspose.Cells.LoadDataFilterOptions enum. Represents the options to filter data when loading workbook from template
## LoadDataFilterOptions enumeration
Represents the options to filter data when loading workbook from template.
```csharp
public enum LoadDataFilterOptions
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | Load nothing for sheet data |
| All | `2147483647` | Load all |
| CellBlank | `1` | Load cells whose value is blank |
| CellString | `2` | Load cells whose value is string |
| CellNumeric | `4` | Load cells whose value is numeric(including datetime) |
| CellError | `8` | Load cells whose value is error |
| CellBool | `16` | Load cells whose value is bool |
| CellValue | `31` | Load cells value(all value types) only |
| Formula | `32` | Load cell formulas. |
| CellData | `67108927` | Load cells data including values, formulas and formatting |
| Chart | `256` | Load charts |
| Shape | `402653696` | Load shapes |
| Drawing | `402653952` | Drawing objects(including Chart, Picture, OleObject and all other drawing objects) |
| MergedArea | `1024` | Load merged cells |
| ConditionalFormatting | `2048` | Load conditional formatting |
| DataValidation | `4096` | Load data validations |
| PivotTable | `8192` | Load pivot tables |
| Table | `16384` | Load tables |
| Hyperlinks | `32768` | Load hyperlinks |
| SheetSettings | `65536` | Load settings for worksheet |
| SheetData | `403701759` | Load all data of worksheet, such as cells data, settings, objects, ...etc. |
| BookSettings | `1048576` | Load settings for workbook |
| Settings | `1114112` | Load settings for workbook and worksheet |
| XmlMap | `2097152` | Load XmlMap |
| Structure | `4194304` | Load structure of the workbook |
| DocumentProperties | `8388608` | Load document properties |
| DefinedNames | `16777216` | Load defined Name objects |
| VBA | `33554432` | Load VBA projects |
| Style | `67108864` | Load styles for cell formatting |
| Picture | `134217728` | Load pictures |
| OleObject | `268435456` | Load OleObjects |
| Revision | `536870912` | Load revision logs |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LoadDataFilterOptionsDemo
{
public static void LoadDataFilterOptionsExample()
{
// Create a new LoadOptions instance
LoadOptions loadOptions = new LoadOptions();
// Create a custom LoadFilter implementation
loadOptions.LoadFilter = new CustomLoadFilter();
// Load the workbook with the specified load options
Workbook workbook = new Workbook("LoadDataFilterOptionsExample_original.xlsx", loadOptions);
// Save the workbook to verify the loaded data
workbook.Save("LoadDataFilterOptionsExample.xlsx");
}
// Custom LoadFilter implementation
private class CustomLoadFilter : LoadFilter
{
public override void StartSheet(Worksheet sheet)
{
// Apply different filter options based on the sheet name
if (sheet.Name == "Sheet1")
{
LoadDataFilterOptions = LoadDataFilterOptions.All;
}
else
{
LoadDataFilterOptions = LoadDataFilterOptions.Structure;
}
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
