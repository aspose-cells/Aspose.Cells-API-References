##PivotTable.AddFieldToArea
PivotTable method. Adds the field to the specific area
## AddFieldToArea(PivotFieldType, string) {#addfieldtoarea_2}
Adds the field to the specific area.
```csharp
public int AddFieldToArea(PivotFieldType fieldType, string fieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| fieldName | String | The name in the base fields. |
### Return Value
The field position in the specific fields.If there is no field named as it, return -1.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Region";
cells["C1"].Value = "Sales";
cells["A2"].Value = "P1";
cells["B2"].Value = "North";
cells["C2"].Value = 1000;
cells["A3"].Value = "P2";
cells["B3"].Value = "South";
cells["C3"].Value = 1500;
cells["A4"].Value = "P3";
cells["B4"].Value = "East";
cells["C4"].Value = 2000;
cells["A5"].Value = "P1";
cells["B5"].Value = "West";
cells["C5"].Value = 1200;
// Add a pivot table
int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivot = sheet.PivotTables[index];
// Add fields to different areas using AddFieldToArea with string field names
pivot.AddFieldToArea(PivotFieldType.Row, "Product");
pivot.AddFieldToArea(PivotFieldType.Column, "Region");
pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh and calculate pivot table
pivot.RefreshData();
pivot.CalculateData();
// Save the workbook
workbook.Save("PivotTableDemo_out.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## AddFieldToArea(PivotFieldType, int) {#addfieldtoarea_1}
Adds the field to the specific area.
```csharp
public int AddFieldToArea(PivotFieldType fieldType, int baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | The fields area type. |
| baseFieldIndex | Int32 | The field index in the base fields. |
### Return Value
The field position in the specific fields.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodAddFieldToAreaWithPivotFieldTypeInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the PivotTable
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Region");
worksheet.Cells["C1"].PutValue("Sales");
for (int i = 2; i <= 10; i++)
{
worksheet.Cells["A" + i].PutValue("Product " + (i % 3 + 1));
worksheet.Cells["B" + i].PutValue("Region " + (i % 2 + 1));
worksheet.Cells["C" + i].PutValue(i * 100);
}
// Add a PivotTable
int pivotTableIndex = worksheet.PivotTables.Add("=A1:C10", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];
// Add fields to areas using AddFieldToArea(PivotFieldType, Int32)
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row field
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column field
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data field
// Save the workbook
workbook.Save("PivotTableDemo_out.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
## AddFieldToArea(PivotFieldType, PivotField) {#addfieldtoarea}
Adds the field to the specific area.
```csharp
public int AddFieldToArea(PivotFieldType fieldType, PivotField pivotField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fieldType | PivotFieldType | the fields area type. |
| pivotField | PivotField | the field in the base fields. |
### Return Value
the field position in the specific fields.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodAddFieldToAreaWithPivotFieldTypePivotFieldDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add a worksheet with source data
Worksheet sourceSheet = workbook.Worksheets[0];
sourceSheet.Name = "Source Data";
// Add sample data
sourceSheet.Cells["A1"].PutValue("Product");
sourceSheet.Cells["B1"].PutValue("Region");
sourceSheet.Cells["C1"].PutValue("Sales");
sourceSheet.Cells["A2"].PutValue("Product A");
sourceSheet.Cells["B2"].PutValue("North");
sourceSheet.Cells["C2"].PutValue(1000);
sourceSheet.Cells["A3"].PutValue("Product B");
sourceSheet.Cells["B3"].PutValue("South");
sourceSheet.Cells["C3"].PutValue(2000);
sourceSheet.Cells["A4"].PutValue("Product A");
sourceSheet.Cells["B4"].PutValue("East");
sourceSheet.Cells["C4"].PutValue(1500);
sourceSheet.Cells["A5"].PutValue("Product B");
sourceSheet.Cells["B5"].PutValue("West");
sourceSheet.Cells["C5"].PutValue(2500);
// Add a pivot table
Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
PivotTableCollection pivotTables = pivotSheet.PivotTables;
string source = "='Source Data'!A1:C5";
int index = pivotTables.Add(source, "A1", "PivotTable");
PivotTable pTable = pivotTables[index];
// Add fields to areas
pTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
pTable.AddFieldToArea(PivotFieldType.Row, 1); // Region
// Add data field
pTable.AddFieldToArea(PivotFieldType.Data, "Sales");
pTable.DataFields[0].Function = ConsolidationFunction.Sum;
pTable.DataFields[0].NumberFormat = "$0.00";
// Add data field to column area using PivotField parameter
if (pTable.DataField != null)
{
pTable.AddFieldToArea(PivotFieldType.Column, pTable.DataField);
}
// Save the workbook
workbook.Save("PivotTableDemo.xlsx");
}
}
}
```
### See Also
* enum [PivotFieldType](../../pivotfieldtype/)
* class [PivotField](../../pivotfield/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
