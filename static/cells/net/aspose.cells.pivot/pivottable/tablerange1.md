##PivotTable.TableRange1
PivotTable property. Returns a CellArea object that represents the range containing the entire PivotTable report but doesnt include page fields. Readonly
## PivotTable.TableRange1 property
Returns a CellArea object that represents the range containing the entire PivotTable report, but doesn't include page fields. Read-only.
```csharp
public CellArea TableRange1 { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyTableRange1Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add a worksheet with sample data
Worksheet dataSheet = workbook.Worksheets[0];
dataSheet.Name = "Data";
dataSheet.Cells["A1"].PutValue("Label");
dataSheet.Cells["B1"].PutValue("Value");
dataSheet.Cells["A2"].PutValue("A");
dataSheet.Cells["B2"].PutValue(10);
dataSheet.Cells["A3"].PutValue("B");
dataSheet.Cells["B3"].PutValue(20);
// Create a pivot table
Worksheet pivotSheet = workbook.Worksheets.Add("Pivot");
int pivotTableIndex = pivotSheet.PivotTables.Add("=Data!A1:B3", "A1", "PivotTable1");
PivotTable pivotTable = pivotSheet.PivotTables[pivotTableIndex];
// Add fields to pivot table
int labelFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Row, "Label");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Configure pivot table
pivotTable.ShowInTabularForm();
pivotTable.RefreshData();
pivotTable.CalculateData();
// Demonstrate TableRange1 property
Console.WriteLine("Pivot Table Range:");
Console.WriteLine($"Start Row: {pivotTable.TableRange1.StartRow}");
Console.WriteLine($"End Row: {pivotTable.TableRange1.EndRow}");
Console.WriteLine($"Start Column: {pivotTable.TableRange1.StartColumn}");
Console.WriteLine($"End Column: {pivotTable.TableRange1.EndColumn}");
// Save the workbook
workbook.Save("PivotTablePropertyTableRange1Demo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
