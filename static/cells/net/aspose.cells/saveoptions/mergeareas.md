##SaveOptions.MergeAreas
SaveOptions property. Indicates whether merge the areas of conditional formatting and validation before saving the file
## SaveOptions.MergeAreas property
Indicates whether merge the areas of conditional formatting and validation before saving the file.
```csharp
public bool MergeAreas { get; set; }
```
### Remarks
The default value is false.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class SaveOptionsPropertyMergeAreasDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill data and create merged cells
worksheet.Cells["A1"].PutValue("Merged Header");
worksheet.Cells["A2"].PutValue("Data 1");
worksheet.Cells["A3"].PutValue("Data 2");
// Merge cells A1:B1
worksheet.Cells.Merge(0, 0, 1, 2);
// Create save options with MergeAreas enabled
XlsSaveOptions saveOptions = new XlsSaveOptions();
saveOptions.MergeAreas = true;
// Save with merged areas optimization
workbook.Save("MergeAreasDemo.xlsx", saveOptions);
}
}
}
```
### See Also
* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
