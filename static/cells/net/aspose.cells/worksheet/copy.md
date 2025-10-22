##Worksheet.Copy
Worksheet method. Copies contents and formats from another worksheet
## Copy(Worksheet) {#copy}
Copies contents and formats from another worksheet.
```csharp
public void Copy(Worksheet sourceSheet)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | Worksheet | Source worksheet. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodCopyWithWorksheetDemo
{
public static void Run()
{
// Create a source workbook with sample data
Workbook sourceWorkbook = new Workbook();
Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
sourceSheet.Cells["A1"].PutValue("Source Worksheet");
// Create a destination workbook
Workbook destWorkbook = new Workbook();
Worksheet destSheet = destWorkbook.Worksheets[0];
// Copy the source worksheet to the destination worksheet
destSheet.Copy(sourceSheet);
// Save the result
destWorkbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Copy(Worksheet, CopyOptions) {#copy_1}
Copies contents and formats from another worksheet.
```csharp
public void Copy(Worksheet sourceSheet, CopyOptions copyOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceSheet | Worksheet | Source worksheet. |
| copyOptions | CopyOptions |  |
### Remarks
You can copy data from another worksheet in the same file or another file. However, this method does not support to copy drawing objects, such as comments, images and charts.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodCopyWithWorksheetCopyOptionsDemo
{
public static void Run()
{
// Create source workbook with sample data
Workbook srcWorkbook = new Workbook();
Worksheet srcSheet = srcWorkbook.Worksheets[0];
srcSheet.Name = "SourceSheet";
srcSheet.Cells["A1"].PutValue("Source Data");
// Create destination workbook
Workbook destWorkbook = new Workbook();
Worksheet destSheet = destWorkbook.Worksheets[0];
destSheet.Name = "DestinationSheet";
// Configure copy options
CopyOptions options = new CopyOptions();
options.ReferToDestinationSheet = true;
// Copy worksheet with options
srcSheet.Copy(destSheet, options);
// Verify the copy operation
Console.WriteLine("Copied cell value: " + destSheet.Cells["A1"].StringValue);
// Save the result
destWorkbook.Save("output.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [CopyOptions](../../copyoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
