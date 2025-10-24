##Class CopyOptions
Aspose.Cells.CopyOptions class. Represents the copy options
## CopyOptions class
Represents the copy options.
```csharp
public class CopyOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [CopyOptions](copyoptions/)() | CopyOptions constructor. |
## Properties
| Name | Description |
| --- | --- |
| [ColumnCharacterWidth](../../aspose.cells/copyoptions/columncharacterwidth/) { get; set; } | Indicates whether copying column width in unit of characters. |
| [CopyInvalidFormulasAsValues](../../aspose.cells/copyoptions/copyinvalidformulasasvalues/) { get; set; } | If the formula is not valid for the dest destination, only copy values. |
| [CopyNames](../../aspose.cells/copyoptions/copynames/) { get; set; } | Indicates whether copying the names. |
| [ExtendToAdjacentRange](../../aspose.cells/copyoptions/extendtoadjacentrange/) { get; set; } | Indicates whether extend ranges when copying the range to adjacent range. |
| [KeepMacros](../../aspose.cells/copyoptions/keepmacros/) { get; set; } | Indicates whether keeping macros; |
| [ReferToDestinationSheet](../../aspose.cells/copyoptions/refertodestinationsheet/) { get; set; } | When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. |
| [ReferToSheetWithSameName](../../aspose.cells/copyoptions/refertosheetwithsamename/) { get; set; } | In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true. |
### Examples
```csharp
using Aspose.Cells;
using System;
namespace AsposeCellsExamples
{
public class CopyOptionsDemo
{
public static void CopyOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some data to the worksheet
sheet.Cells["A1"].PutValue("Hello");
sheet.Cells["A2"].PutValue("World");
// Create a new workbook to copy data into
Workbook destWorkbook = new Workbook();
Worksheet destSheet = destWorkbook.Worksheets[0];
// Create a CopyOptions object
CopyOptions copyOptions = new CopyOptions
{
KeepMacros = true,
ExtendToAdjacentRange = true,
CopyNames = true,
CopyInvalidFormulasAsValues = true,
ColumnCharacterWidth = true,
ReferToSheetWithSameName = true,
ReferToDestinationSheet = true
};
// Copy the data from the source worksheet to the destination worksheet
destSheet.Cells.CopyRows(sheet.Cells, 0, 0, 2, copyOptions);
// Save the destination workbook
destWorkbook.Save("CopyOptionsExample.xlsx");
destWorkbook.Save("CopyOptionsExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
