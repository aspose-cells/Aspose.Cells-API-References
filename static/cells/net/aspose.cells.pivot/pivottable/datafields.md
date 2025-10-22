##PivotTable.DataFields
PivotTable property. Gets a PivotField object that represents all the data fields in a PivotTable. Readonly.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area
## PivotTable.DataFields property
Gets a PivotField object that represents all the data fields in a PivotTable. Read-only.It would be init only when there are two or more data fields in the DataPiovtFiels. It only use to add DataPivotField to the PivotTable row/column area . Default is in row area.
```csharp
public PivotFieldCollection DataFields { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyDataFieldsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 20;
cells["A4"].Value = "Banana";
cells["B4"].Value = 15;
// Add a pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Access data fields and demonstrate functionality
PivotFieldCollection dataFields = pivotTable.DataFields;
if (dataFields.Count > 0)
{
PivotField dataField = dataFields[0];
Console.WriteLine("Data Field Name: " + dataField.Name);
Console.WriteLine("Data Field Function: " + dataField.Function);
}
// Save the workbook
workbook.Save("PivotTableDataFieldsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
