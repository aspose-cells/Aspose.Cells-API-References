##Cell.SetSharedFormula
Cell method. Sets a formula to a range of cells
## SetSharedFormula(string, int, int, bool, bool) {#setsharedformula_3}
Sets a formula to a range of cells.
```csharp
[Obsolete("Use FormulaParseOptions for more options instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber, bool isR1C1,
bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| isR1C1 | Boolean | whether the formula is R1C1 formula |
| isLocal | Boolean | whether the formula is locale formatted |
### Remarks
NOTE: This class is now obsolete. Instead, please use Cell.SetSharedFormula(string,int,int,FormulaParseOptions). This property will be removed 12 months later since December 2019. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodSetSharedFormulaWithStringInt32Int32BooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Populate sample data in column A
for (int row = 0; row < 5; row++)
{
cells[row, 0].Value = row + 1; // A1-A5: 1-5
}
// Get target cell B1 to set shared formula
Cell targetCell = cells[0, 1]; // B1
try
{
// Set shared formula to calculate square of values in column A
// Parameters: (formula, rowCount=5, columnCount=1, isR1C1=false, isLocal=false)
#pragma warning disable 0618 // Disable obsolete warning for demonstration
targetCell.SetSharedFormula("=A1^2", 5, 1, false, false);
#pragma warning restore 0618
// Verify formula propagation
Console.WriteLine($"B1 formula: {targetCell.Formula}");
Console.WriteLine($"B5 formula: {cells[4, 1].Formula}");
// Calculate workbook to refresh formula results
workbook.CalculateFormula();
Console.WriteLine($"A1 value: {cells["A1"].Value}");
Console.WriteLine($"A5 value: {cells["A5"].Value}");
Console.WriteLine($"B1 value: {targetCell.Value}");
Console.WriteLine($"B5 value: {cells[4, 1].Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Error setting shared formula: {ex.Message}");
return;
}
// Save the modified workbook
workbook.Save("SetSharedFormulaDemo.xlsx");
Console.WriteLine("Spreadsheet saved successfully.");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetSharedFormula(string, int, int) {#setsharedformula}
Sets shared formulas to a range of cells.
```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodSetSharedFormulaWithStringInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set a shared formula in column B starting from B1 to B20
cells["B1"].SetSharedFormula("=C1*2", 20, 1);
// Set some values in column C to demonstrate the formula calculation
for (int i = 0; i < 20; i++)
{
cells[i, 2].PutValue(i + 1); // Column C values (C1=1, C2=2...)
}
// Calculate formulas
workbook.CalculateFormula();
// Output results for verification
for (int i = 0; i < 5; i++) // Display first 5 results
{
Console.WriteLine($"B{i+1} value: {cells[i, 1].Value}");
}
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetSharedFormula(string, int, int, FormulaParseOptions) {#setsharedformula_1}
Sets shared formulas to a range of cells.
```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber,
FormulaParseOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample data in column A
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
// Get target cell where we'll set the shared formula
Cell targetCell = worksheet.Cells["B1"];
try
{
// Create formula parse options with default settings
FormulaParseOptions options = new FormulaParseOptions();
// Set shared formula for 3 rows and 2 columns starting from B1
targetCell.SetSharedFormula("=A1*2", 3, 2, options);
Console.WriteLine("Shared formula set successfully for B1:C3 range");
Console.WriteLine("B1 formula: " + worksheet.Cells["B1"].Formula);
Console.WriteLine("C3 formula: " + worksheet.Cells["C3"].Formula);
workbook.CalculateFormula();
Console.WriteLine("B3 value: " + worksheet.Cells["B3"].Value);
Console.WriteLine("B1 value: " + worksheet.Cells["B1"].Value);
Console.WriteLine("C3 value: " + worksheet.Cells["C3"].Value);
}
catch (Exception ex)
{
Console.WriteLine($"Error setting shared formula: {ex.Message}");
}
// Save the modified workbook
workbook.Save("SetSharedFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## SetSharedFormula(string, int, int, FormulaParseOptions, object[][]) {#setsharedformula_2}
Sets shared formulas to a range of cells.
```csharp
public void SetSharedFormula(string sharedFormula, int rowNumber, int columnNumber,
FormulaParseOptions options, object[][] values)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sharedFormula | String | Shared formula. |
| rowNumber | Int32 | Number of rows to populate the formula. |
| columnNumber | Int32 | Number of columns to populate the formula. |
| options | FormulaParseOptions | Options for parsing the formula. |
| values | Object[][] | values for those cells with given shared formula |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Collections;
public class CellMethodSetSharedFormulaWithStringInt32Int32FormulaParseOpDemo1
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample value in cell A1
worksheet.Cells["A1"].PutValue(5);
// Get target cell B2 where the shared formula will be set
Cell cell = worksheet.Cells["B2"];
try
{
// Define shared formula parameters
string formula = "=A1*2";
int totalRows = 2;
int totalColumns = 2;
FormulaParseOptions parseOptions = new FormulaParseOptions();
object[][] presetValues = new object[2][]
{
new object[] { 10, 10 },
new object[] { 10, 10 }
};
// Set shared formula for 2x2 range starting at B2 with preset values
cell.SetSharedFormula(formula, totalRows, totalColumns, parseOptions, presetValues);
Console.WriteLine("Shared formula set successfully. Cells B2:C3 contain values 10");
workbook.CalculateFormula();
Aspose.Cells.Range range = worksheet.Cells.CreateRange("B2", "C3");
IEnumerator iter = range.GetEnumerator();
while(iter.MoveNext())
{
Cell temp = (Cell)iter.Current;
Console.WriteLine(temp.Name + "  " + temp.Value);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error setting shared formula: {ex.Message}");
}
// Save the modified workbook
workbook.Save("SetSharedFormulaDemo.xlsx");
}
}
}
```
### See Also
* class [FormulaParseOptions](../../formulaparseoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
