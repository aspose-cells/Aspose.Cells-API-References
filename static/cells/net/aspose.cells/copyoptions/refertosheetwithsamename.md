##CopyOptions.ReferToSheetWithSameName
CopyOptions property. In ms excel when copying formulas which refer to other worksheets while copying a worksheet to another one the copied formulas should refer to source workbook. However for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook such as when those worksheets have been copied before this copy operation then this property should be kept as true
## CopyOptions.ReferToSheetWithSameName property
In ms excel, when copying formulas which refer to other worksheets while copying a worksheet to another one, the copied formulas should refer to source workbook. However, for some situations user may need the copied formulas refer to worksheets with the same name in the same workbook, such as when those worksheets have been copied before this copy operation, then this property should be kept as true.
```csharp
public bool ReferToSheetWithSameName { get; set; }
```
### Remarks
The default value is true.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CopyOptionsPropertyReferToSheetWithSameNameDemo
{
public static void Run()
{
// Create a template workbook with sample data
Workbook templateWorkbook = new Workbook();
Worksheet templateSheet1 = templateWorkbook.Worksheets[0];
templateSheet1.Name = "Data";
templateSheet1.Cells["A1"].PutValue("Value");
templateSheet1.Cells["A2"].PutValue(10);
templateSheet1.Cells["A3"].PutValue(20);
Worksheet templateSheet2 = templateWorkbook.Worksheets.Add("Summary");
templateSheet2.Cells["B2"].Formula = "=SUM(Data!A2:A3)";
// Create output workbook
Workbook outputWorkbook = new Workbook();
outputWorkbook.Worksheets.Clear();
// Copy worksheets with ReferToSheetWithSameName enabled
foreach (Worksheet sheet in templateWorkbook.Worksheets)
{
outputWorkbook.Worksheets.Add(sheet.Name);
CopyOptions options = new CopyOptions();
options.ReferToSheetWithSameName = true;
outputWorkbook.Worksheets[sheet.Name].Copy(sheet, options);
}
// Verify the formula references the correct sheet
Console.WriteLine("Formula in output workbook: " +
outputWorkbook.Worksheets["Summary"].Cells["B2"].Formula);
}
}
}
```
### See Also
* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
