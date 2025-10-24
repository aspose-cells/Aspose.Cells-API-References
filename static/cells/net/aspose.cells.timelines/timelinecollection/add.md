##TimelineCollection.Add
TimelineCollection method. Add a new Timeline using PivotTable as data source
## Add(PivotTable, int, int, string) {#add_2}
Add a new Timeline using PivotTable as data source
```csharp
public int Add(PivotTable pivot, int row, int column, string baseFieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Timeline range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |
### Return Value
The new add Timeline index
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class TimelineCollectionMethodAddWithPivotTableInt32Int32StringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Date";
cells["C1"].Value = "Sales";
cells["A2"].Value = "P1";
cells["B2"].Value = new DateTime(2023, 1, 1);
cells["C2"].Value = 100;
cells["A3"].Value = "P2";
cells["B3"].Value = new DateTime(2023, 1, 2);
cells["C3"].Value = 150;
cells["A4"].Value = "P1";
cells["B4"].Value = new DateTime(2023, 1, 3);
cells["C4"].Value = 200;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int pivotIndex = pivotTables.Add("A1:C4", "E3", "PivotTable1");
PivotTable pivot = pivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, 0);
pivot.AddFieldToArea(PivotFieldType.Column, 1);
pivot.AddFieldToArea(PivotFieldType.Data, 2);
// Add timeline connected to the pivot table
sheet.Timelines.Add(pivot, 10, 5, "Date");
// Save workbook
workbook.Save("TimelineDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
## Add(PivotTable, string, string) {#add_5}
Add a new Timeline using PivotTable as data source
```csharp
public int Add(PivotTable pivot, string destCellName, string baseFieldName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell name in the upper-left corner of the Timeline range. |
| baseFieldName | String | The name of PivotField in PivotTable.BaseFields |
### Return Value
The new add Timeline index
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class TimelineCollectionMethodAddWithPivotTableStringStringDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].PutValue("Date");
sheet.Cells["A2"].PutValue(DateTime.Now);
sheet.Cells["A3"].PutValue(DateTime.Now.AddDays(1));
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["B2"].PutValue(100);
sheet.Cells["B3"].PutValue(200);
// Add pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B3", "C1", "PivotTable1");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, 0);
// Add timeline connected to the pivot table
sheet.Timelines.Add(pivot, "E1", "Date");
// Save the workbook
workbook.Save("TimelineDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
## Add(PivotTable, int, int, int) {#add_1}
Add a new Timeline using PivotTable as data source
```csharp
public int Add(PivotTable pivot, int row, int column, int baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Timeline range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldIndex | Int32 | The index of PivotField in PivotTable.BaseFields |
### Return Value
The new add Timeline index
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class TimelineCollectionMethodAddWithPivotTableInt32Int32Int32Demo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 5;
cells["A4"].Value = "Banana";
cells["B4"].Value = 7;
// Add pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivot = sheet.PivotTables[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, 0);
pivot.AddFieldToArea(PivotFieldType.Data, 1);
// Add timeline control
sheet.Timelines.Add(pivot, 15, 5, 1);
}
}
}
```
### See Also
* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
## Add(PivotTable, string, int) {#add_4}
Add a new Timeline using PivotTable as data source
```csharp
public int Add(PivotTable pivot, string destCellName, int baseFieldIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell name in the upper-left corner of the Timeline range. |
| baseFieldIndex | Int32 | The index of PivotField in PivotTable.BaseFields |
### Return Value
The new add Timeline index
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Timelines;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class TimelineCollectionMethodAddWithPivotTableStringInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data to the worksheet
Cells cells = sheet.Cells;
cells["A1"].PutValue("Date");
cells["B1"].PutValue("Product");
cells["C1"].PutValue("Sales");
cells["A2"].PutValue(new DateTime(2023, 1, 1));
cells["B2"].PutValue("A");
cells["C2"].PutValue(100);
cells["A3"].PutValue(new DateTime(2023, 1, 2));
cells["B3"].PutValue("B");
cells["C3"].PutValue(200);
cells["A4"].PutValue(new DateTime(2023, 1, 3));
cells["B4"].PutValue("A");
cells["C4"].PutValue(150);
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Date");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Refresh pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Find base field index for "Date" field
int dateFieldIndex = -1;
for (int i = 0; i < pivotTable.BaseFields.Count; i++)
{
if (pivotTable.BaseFields[i].Name == "Date")
{
dateFieldIndex = i;
break;
}
}
// Add timeline using the found index
if (dateFieldIndex >= 0)
{
sheet.Timelines.Add(pivotTable, "H2", dateFieldIndex);
}
// Save the result
workbook.Save("TimelineCollectionMethodAddWithPivotTableStringInt32Demo_output.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
## Add(PivotTable, int, int, PivotField) {#add}
Add a new Timeline using PivotTable as data source
```csharp
public int Add(PivotTable pivot, int row, int column, PivotField baseField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| row | Int32 | Row index of the cell in the upper-left corner of the Timeline range. |
| column | Int32 | Column index of the cell in the upper-left corner of the Timeline range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |
### Return Value
The new add Timeline index
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Date";
cells["C1"].Value = "Sales";
cells["A2"].Value = "P1";
cells["B2"].Value = new DateTime(2023, 1, 1);
cells["C2"].Value = 100;
cells["A3"].Value = "P2";
cells["B3"].Value = new DateTime(2023, 1, 2);
cells["C3"].Value = 150;
cells["A4"].Value = "P1";
cells["B4"].Value = new DateTime(2023, 2, 1);
cells["C4"].Value = 200;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int index = pivotTables.Add("A1:C4", "E3", "PivotTable1");
PivotTable pivot = pivotTables[index];
// Add pivot fields
pivot.AddFieldToArea(PivotFieldType.Row, pivot.BaseFields[0]);
pivot.AddFieldToArea(PivotFieldType.Column, pivot.BaseFields[1]);
pivot.AddFieldToArea(PivotFieldType.Data, pivot.BaseFields[2]);
// Add timeline using the pivot table
sheet.Timelines.Add(pivot, 20, 5, pivot.BaseFields[1]);
// Save the workbook
workbook.Save("TimelineCollectionMethodAddWithPivotTableInt32Int32PivotFieldDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
## Add(PivotTable, string, PivotField) {#add_3}
Add a new Timeline using PivotTable as data source
```csharp
public int Add(PivotTable pivot, string destCellName, PivotField baseField)
```
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | PivotTable | PivotTable object |
| destCellName | String | The cell name in the upper-left corner of the Timeline range. |
| baseField | PivotField | The PivotField in PivotTable.BaseFields |
### Return Value
The new add Timeline index
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class TimelineCollectionMethodAddWithPivotTableStringPivotFieldDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 20;
cells["A4"].Value = "Banana";
cells["B4"].Value = 15;
// Create pivot table
PivotTableCollection pivotTables = sheet.PivotTables;
int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivot = pivotTables[index];
pivot.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivot.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Add timeline using pivot table as data source
sheet.Timelines.Add(pivot, "i10", pivot.BaseFields[0]);
}
}
}
```
### See Also
* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [PivotField](../../../aspose.cells.pivot/pivotfield/)
* class [TimelineCollection](../)
* namespace [Aspose.Cells.Timelines](../../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../../)
