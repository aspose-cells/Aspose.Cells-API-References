##Workbook.Combine
Workbook method. Combines another Workbook object
## Workbook.Combine method
Combines another Workbook object.
```csharp
public void Combine(Workbook secondWorkbook)
```
| Parameter | Type | Description |
| --- | --- | --- |
| secondWorkbook | Workbook | Another Workbook object. |
### Remarks
Merge Excel, ODS , CSV and other files to one file.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCombineWithWorkbookDemo
{
public static void Run()
{
// Create source workbook
Workbook sourceWorkbook = new Workbook();
sourceWorkbook.Worksheets[0].Cells["A1"].PutValue("Source Data");
// Create destination workbook
Workbook destWorkbook = new Workbook(FileFormatType.Xlsx);
destWorkbook.Worksheets[0].Cells["B2"].PutValue("Destination Data");
// Combine the workbooks
destWorkbook.Combine(sourceWorkbook);
// Save the combined workbook
destWorkbook.Save("CombinedWorkbook.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
