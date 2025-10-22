##CopyOptions.ReferToDestinationSheet
CopyOptions property. When copying the range in the same file and the chart refers to the source sheet False means the copied charts data source will not be changed. True means the copied charts data source refers to the destination sheet
## CopyOptions.ReferToDestinationSheet property
When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet.
```csharp
public bool ReferToDestinationSheet { get; set; }
```
### Remarks
The default value is false, it works as MS Excel. For example: if copying a chart with the data source "sheet1!A1:B10" from worksheet "sheet1 to other worksheet "sheet2", The data source will be changed as "sheet2!A1:B10"
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CopyOptionsPropertyReferToDestinationSheetDemo
{
public static void Run()
{
// Create source workbook with sample data
Workbook sourceWorkbook = new Workbook();
Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
sourceSheet.Cells["A1"].PutValue("Source Data");
sourceSheet.Cells["B1"].PutValue(100);
sourceSheet.Cells["A2"].PutValue("=SUM(B1)");
// Create destination workbook
Workbook destWorkbook = new Workbook();
Worksheet destSheet = destWorkbook.Worksheets.Add("DestinationSheet");
// Set copy options with ReferToDestinationSheet
CopyOptions copyOptions = new CopyOptions();
copyOptions.ReferToDestinationSheet = true;
// Copy worksheet with the options
destSheet.Copy(sourceSheet, copyOptions);
// Save the result
destWorkbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
