##Cell.SetArrayFormula
Cell method. Sets an array formula to a range of cells
## SetArrayFormula(string, int, int, bool, bool) {#setarrayformula_3}
Sets an array formula to a range of cells.
```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber, bool isR1C1,
bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |
| isR1C1 | Boolean | whether the formula is R1C1 formula |
| isLocal | Boolean | whether the formula is locale formatted |
### Remarks
NOTE: This class is now obsolete. Instead, please use Cell.SetArrayFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetArrayFormula(string, int, int) {#setarrayformula}
Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells.
```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodSetArrayFormulaWithStringInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
Cell cell = cells["A1"];
cell.SetArrayFormula("=FREQUENCY({\"79\",\"85\",\"78\",\"85\",\"50\",\"81\",\"95\",\"88\",\"97\"},{70,79,89})", 4, 1);
workbook.CalculateFormula();
for (int i = 0; i < 4; i++)
{
Console.WriteLine($"Cell A{i+1} value: {cells[i, 0].IntValue}");
}
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetArrayFormula(string, int, int, FormulaParseOptions) {#setarrayformula_1}
Sets an array formula to a range of cells.
```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber,
FormulaParseOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodSetArrayFormulaWithStringInt32Int32FormulaParseOpDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Put sample data in cells C1:E1
cells["C1"].PutValue(10);
cells["D1"].PutValue(20);
cells["E1"].PutValue(30);
// Set array formula in cell A1 that will spill to 2 rows and 3 columns
cells["A1"].SetArrayFormula("=TRANSPOSE(C1:E1)", 2, 1, new FormulaParseOptions());
// Calculate formulas
workbook.CalculateFormula();
// Output the results
Console.WriteLine("Array formula results:");
for (int row = 0; row < 2; row++)
{
for (int col = 0; col < 3; col++)
{
Cell cell = cells[row, col];
Console.WriteLine($"Cell {cell.Name}: {cell.Value}");
}
}
}
}
}
```
### See Also
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetArrayFormula(string, int, int, FormulaParseOptions, object[][]) {#setarrayformula_2}
Sets an array formula to a range of cells.
```csharp
public void SetArrayFormula(string arrayFormula, int rowNumber, int columnNumber,
FormulaParseOptions options, object[][] values)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | String | Array formula. |
| rowNumber | Int32 | Number of rows to populate result of the array formula. |
| columnNumber | Int32 | Number of columns to populate result of the array formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| values | Object[][] | values for those cells with given array formula |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodSetArrayFormulaWithStringInt32Int32FormulaParseOpDemo2
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells[0, 0]; // Target cell A1
// Prepare array formula parameters
string arrayFormula = "{1,2;3,4;5,6}"; // 3x2 array formula
int rowNumber = 3;
int columnNumber = 2;
FormulaParseOptions options = new FormulaParseOptions();
object[][] values = new object[3][]
{
new object[] { 1, 2 },
new object[] { 3, 4 },
new object[] { 5, 6 }
};
try
{
// Set array formula with predefined values
cell.SetArrayFormula(arrayFormula, rowNumber, columnNumber, options, values);
Console.WriteLine("Array formula set successfully in A1:B3");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetArrayFormula: {ex.Message}");
}
// Save the workbook
workbook.Save("SetArrayFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
