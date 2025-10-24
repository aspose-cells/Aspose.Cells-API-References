##Cell.SetTableFormula
Cell method. Create twovariable data table for given range starting from this cell
## SetTableFormula(int, int, string, string, object[][]) {#settableformula_3}
Create two-variable data table for given range starting from this cell.
```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string rowInputCell,
string columnInputCell, object[][] values)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| rowInputCell | String | the row input cell |
| columnInputCell | String | the column input cell |
| values | Object[][] | values for cells in table formula range |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodSetTableFormulaWithInt32Int32StringStringObjectArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = workbook.Worksheets[0].Cells;
cells[1, 1].Formula = "=A1+A2";
cells[1, 2].PutValue(2);
cells[1, 3].PutValue(3);
cells[2, 1].PutValue(2);
cells[3, 1].PutValue(3);
cells[4, 1].PutValue(4);
// Target cell where table formula will be set
Cell targetCell = worksheet.Cells["C3"];
// Prepare parameters for SetTableFormula
int rowNumber = 3;
int columnNumber = 2;
string rowInputCell = "A1";
string columnInputCell = "A2";
object[][] values = new object[][]
{
new object[] { 1, 2 },    // Row 1 data
new object[] { 3, 4 },    // Row 2 data
new object[] { 5, 6 }     // Row 3 data
};
try
{
// Set the table formula on the target cell
targetCell.SetTableFormula(rowNumber, columnNumber, rowInputCell, columnInputCell, values);
// Calculate workbook formulas to refresh results
workbook.CalculateFormula();
Console.WriteLine("Table formula set successfully. Check D1:" + targetCell.StringValue);
}
catch (Exception ex)
{
Console.WriteLine($"Error setting table formula: {ex.Message}");
}
// Save the modified workbook
workbook.Save("SetTableFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetTableFormula(int, int, string, bool, object[][]) {#settableformula_2}
Create one-variable data table for given range starting from this cell.
```csharp
public void SetTableFormula(int rowNumber, int columnNumber, string inputCell, bool isRowInput,
object[][] values)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| inputCell | String | the input cell |
| isRowInput | Boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | Object[][] | values for cells in table formula range |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodSetTableFormulaWithInt32Int32StringBooleanObjectDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
cells[1, 1].Formula = "=A1+A2";
cells[1, 2].PutValue(100000);
cells[1, 3].PutValue(0.05);
cells[1, 4].PutValue(2);
cells[2, 1].PutValue(360);
cells[3, 1].PutValue(30);
cells[4, 1].PutValue(40);
try
{
// Prepare parameters for SetTableFormula
int rowCount = 3;
int colCount = 3;
object[][] inputValues = new object[][]
{
new object[] { 0.05, 0.06, 0.07 },
new object[] { 1000, 2000, 3000 },
new object[] { 100, 200, 300 }
};
// Get target cell for data table (C3)
Cell tableCell = worksheet.Cells["C3"];
// Call SetTableFormula with interest rate variations
tableCell.SetTableFormula(
rowNumber: rowCount,
columnNumber: colCount,
inputCell: "A1",
isRowInput: true,
values: inputValues
);
// Calculate formulas to refresh table results
workbook.CalculateFormula();
Console.WriteLine("Data table created successfully with varying interest rates");
}
catch (Exception ex)
{
Console.WriteLine($"Error creating data table: {ex.Message}");
}
// Save the modified workbook
workbook.Save("SetTableFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetTableFormula(int, int, int, int, int, int, object[][]) {#settableformula_1}
Create two-variable data table for given range starting from this cell.
```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfRowInputCell,
int columnIndexOfRowInputCell, int rowIndexOfColumnInputCell, int columnIndexOfColumnInputCell,
object[][] values)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| rowIndexOfRowInputCell | Int32 | row index of the row input cell |
| columnIndexOfRowInputCell | Int32 | column index of the row input cell |
| rowIndexOfColumnInputCell | Int32 | row index of the column input cell |
| columnIndexOfColumnInputCell | Int32 | column index of the column input cell |
| values | Object[][] | values for cells in table formula range |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodSetTableFormulaWithInt32Int32Int32Int32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells[1, 1].Formula = "=A1+A2";
cells[1, 2].PutValue(2);
cells[1, 3].PutValue(3);
cells[1, 4].PutValue(4);
cells[2, 1].PutValue(2);
cells[3, 1].PutValue(3);
cells[4, 1].PutValue(4);
Cell formulaCell = cells[2, 2];
// Prepare input values for data table (interest rates and loan amounts)
object[][] tableValues = new object[3][];
tableValues[0] = new object[] { 0.05, 0.06, 0.07 };
tableValues[1] = new object[] { 1000, 2000, 3000 };
tableValues[2] = new object[] { 100, 200, 300 };
try
{
// Set table formula with 3x3 data table dimensions and input cell offsets
formulaCell.SetTableFormula(
rowNumber: 3,
columnNumber: 3,
rowIndexOfRowInputCell: 0,
columnIndexOfRowInputCell: 0,
rowIndexOfColumnInputCell: 1,
columnIndexOfColumnInputCell: 0,
values: tableValues
);
workbook.CalculateFormula();
Console.WriteLine("Data table formula set successfully. Check B2:D4 in output.");
}
catch (Exception ex)
{
Console.WriteLine($"Error setting table formula: {ex.Message}");
}
workbook.Save("CellTableFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetTableFormula(int, int, int, int, bool, object[][]) {#settableformula}
Create one-variable data table for given range starting from this cell.
```csharp
public void SetTableFormula(int rowNumber, int columnNumber, int rowIndexOfInputCell,
int columnIndexOfInputCell, bool isRowInput, object[][] values)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| rowIndexOfInputCell | Int32 | row index of the input cell |
| columnIndexOfInputCell | Int32 | column index of the input cell |
| isRowInput | Boolean | Indicates whether the input cell is a row input cell(true) or a column input cell(false). |
| values | Object[][] | values for cells in table formula range |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodSetTableFormulaWithInt32Int32Int32Int32BooleanObjDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = workbook.Worksheets[0].Cells;
cells[1, 1].Formula = "=A1+A2";
cells[1, 2].PutValue(20);
cells[1, 3].PutValue(30);
cells[2, 1].PutValue(20);
cells[3, 1].PutValue(30);
cells[4, 1].PutValue(40);
// Create sample data array for table formula parameters
object[][] inputValues = new object[][]
{
new object[] { 10, 20 },
new object[] { 30, 40 },
new object[] { 50, 60 }
};
// Get target cell to apply table formula
Cell formulaCell = worksheet.Cells[2, 2];
try
{
// Set table formula with:
// 3 rows, 2 columns, input cell at A1 (0,0),
// row input type, and sample values
formulaCell.SetTableFormula(
rowNumber: 3,
columnNumber: 2,
rowIndexOfInputCell: 0,
columnIndexOfInputCell: 0,
isRowInput: true,
values: inputValues
);
workbook.CalculateFormula();
Console.WriteLine("Table formula applied successfully. " +
"Saved workbook with 3x2 table formula at C3.");
}
catch (Exception ex)
{
Console.WriteLine($"Error setting table formula: {ex.Message}");
}
// Save the modified workbook
workbook.Save("TableFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
