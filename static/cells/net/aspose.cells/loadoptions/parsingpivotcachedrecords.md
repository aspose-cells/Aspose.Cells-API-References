##LoadOptions.ParsingPivotCachedRecords
LoadOptions property. Indicates whether parsing pivot cached records when loading the file. The default value is false
## LoadOptions.ParsingPivotCachedRecords property
Indicates whether parsing pivot cached records when loading the file. The default value is false.
```csharp
public bool ParsingPivotCachedRecords { get; set; }
```
### Remarks
Only applies for Excel Xlsx, Xltx, Xltm , Xlsm and xlsb file
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyParsingPivotCachedRecordsDemo
{
public static void Run()
{
// Create CSV load options
TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv);
// Enable parsing pivot cached records
loadOptions.ParsingPivotCachedRecords = true;
// Load workbook with the options
Workbook workbook = new Workbook("example.csv", loadOptions);
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Name = "PivotData";
// Create pivot table (demonstrating the property is set)
int pivotIndex = worksheet.PivotTables.Add("A1:C10", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Save the workbook
workbook.Save("PivotTableOutput.xlsx");
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
