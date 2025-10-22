##AutoFitterOptions.AutoFitMergedCells
AutoFitterOptions property. Indicates whether auto fit row height when the cells is merged in a row. The default value is false
## AutoFitterOptions.AutoFitMergedCells property
Indicates whether auto fit row height when the cells is merged in a row. The default value is false.
```csharp
[Obsolete("Use AutoFitterOptions.AutoFitMergedCellsType property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AutoFitMergedCells { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use AutoFitterOptions.AutoFitMergedCellsType property, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFitterOptionsPropertyAutoFitMergedCellsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data and merge cells
worksheet.Cells["A1"].PutValue("This is a test of AutoFitMergedCells property");
worksheet.Cells.Merge(0, 0, 3, 3); // Merge cells A1:C3
// Create AutoFitterOptions and set AutoFitMergedCells
AutoFitterOptions options = new AutoFitterOptions();
options.AutoFitMergedCells = true;
// AutoFit rows with merged cells
worksheet.AutoFitRows(options);
// Save the workbook
workbook.Save("AutoFitMergedCellsExample.xlsx");
}
}
}
```
### See Also
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
