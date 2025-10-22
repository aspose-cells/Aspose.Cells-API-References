##AutoFitterOptions.AutoFitMergedCellsType
AutoFitterOptions property. Gets and set the type of auto fitting row height of merged cells
## AutoFitterOptions.AutoFitMergedCellsType property
Gets and set the type of auto fitting row height of merged cells.
```csharp
public AutoFitMergedCellsType AutoFitMergedCellsType { get; set; }
```
### Remarks
Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AutoFitterOptionsPropertyAutoFitMergedCellsTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data and merge cells
worksheet.Cells["A1"].PutValue("This is a sample text for merged cells auto-fit demonstration");
worksheet.Cells.Merge(0, 0, 3, 2); // Merge A1:B3
// AutoFit rows with AutoFitMergedCellsType.EachLine
worksheet.AutoFitRows(new AutoFitterOptions
{
AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
});
// AutoFit columns with AutoFitMergedCellsType.EachLine
worksheet.AutoFitColumns(new AutoFitterOptions
{
AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine,
AutoFitWrappedTextType = AutoFitWrappedTextType.Paragraph
});
// Save the workbook
workbook.Save("AutoFitMergedCellsDemo.xlsx");
}
}
}
```
### See Also
* enum [AutoFitMergedCellsType](../../autofitmergedcellstype/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
