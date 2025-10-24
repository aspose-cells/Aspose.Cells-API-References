##Enum AccessCacheOptions
Aspose.Cells.AccessCacheOptions enum. Cache options for data access. Can be combined with  operator for multiple options together
## AccessCacheOptions enumeration
Cache options for data access. Can be combined with &#x7C; operator for multiple options together.
```csharp
[Flags]
public enum AccessCacheOptions
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No cache for any data access. |
| All | `FFFFFFFFFFFFFFFF` | Apply all possible optimizations for all kinds of data access in the workbook. All settings and data should not be changed during the optimized access. |
| PositionAndSize | `3` | Apply possible optimization for getting object(such as Shape)'s position and size. Row height and column width settings should not be changed during the optimized access. |
| CellsData | `9` | Apply possible optimization for getting cells' values. Cells data(data and settings of Cell, Row) should not be changed during the optimized access, no new Cell/Row objects should be created either(such as by [`Item`](../cells/item/)). |
| CellDisplay | `100086` | Apply possible optimization for getting display-related results of cells([`DisplayStringValue`](../cell/displaystringvalue/), [`GetStyle`](../cell/getstyle/), [`GetDisplayStyle`](../cell/getdisplaystyle/), etc.). Cells data and style-related objects(Cell/Row/Column styles, column width, etc.) should not be changed during the optimized access. |
| GetFormula | `200000` | Apply possible optimization for getting formulas. All data and settings which may affect the formula expression(Worksheet's name, Name's text, table's column, etc.) should not be changed during the optimized access. |
| SetFormula | `400000` | Apply possible optimization for setting formulas. All data and settings which may affect the formula expression(Worksheet's name, Name's text, table's column, etc.) should not be changed during the optimized access. |
| CalculateFormula | `800009` | Apply possible optimization for calculating formulas. Cells data should not be changed during the optimized access, none new objects(Cell, Row, etc.) should be created either(such as by [`Item`](../cells/item/)). |
| ConditionalFormatting | `1000009` | Apply possible optimization for getting formatting result of conditional formattings. All data and settings which may affect the result of conditional formattings(settings of conditional formattings, dependent cell values, etc.) should not be changed during the optimized access. |
| Validation | `2000009` | Apply possible optimization for getting validation result. All data and settings which may affect the result of validation(settings of the validation, dependent cell values, etc.) should not be changed during the optimized access. |
### Remarks
For some features, accessing large dataset requires a lot of repeated and complicated operations such as search, calculation, ...etc and those operations will take a lot of extra time. For common situations, all dependent data remains unchanged during the access, so some caches can be built and used to improve the access performance. For this purpose, we provide this API so that user can specify which kind of data access needs to be optimized by possible caching mechanism.  Please note, for different options, different data set may be required to be "read-only". And performance of accessing data depends on many aspects, the use of caching mechanism does not guarantee that performance will be improved. For some situations, such as the dataset to be accessed is small, using cache may cause even more time because caching itself also needs certain extra time.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class AccessCacheOptionsDemo
{
public static void AccessCacheOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Start access cache with specific options
workbook.StartAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);
// Perform some operations that benefit from caching
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 10; j++)
{
worksheet.Cells[i, j].PutValue(i + j);
}
}
// Close access cache
workbook.CloseAccessCache(AccessCacheOptions.PositionAndSize | AccessCacheOptions.CellsData);
// Save the workbook
workbook.Save("AccessCacheOptionsExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
