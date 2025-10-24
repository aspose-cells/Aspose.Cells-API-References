##Cells.ImportArray
Cells method.
## ImportArray(string[], int, int) {#importarray_4}
```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn)
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportArray(string[], int, int, bool) {#importarray_5}
Imports an array of string into a worksheet.
```csharp
public void ImportArray(string[] stringArray, int firstRow, int firstColumn, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| stringArray | String[] | String array. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| isVertical | Boolean | Specifies to import data vertically or horizontally. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodImportArrayWithStringInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare string array data
string[] fruitArray = new string[] { "Apple", "Banana", "Cherry", "Date", "Elderberry" };
try
{
// Call ImportArray with parameters: (String[], Int32, Int32, Boolean)
// Start importing at row 2 (3rd row), column 1 (B column), vertically
worksheet.Cells.ImportArray(fruitArray, 2, 1, true);
Console.WriteLine("Imported string array vertically starting from cell B3:");
foreach (string fruit in fruitArray)
{
Console.WriteLine(fruit);
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
}
// Save the result
workbook.Save("CellsMethodImportArrayWithStringInt32Int32BooleanDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportArray(int[], int, int) {#importarray_2}
```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn)
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportArray(int[], int, int, bool) {#importarray_3}
Imports an array of integer into a worksheet.
```csharp
public void ImportArray(int[] intArray, int firstRow, int firstColumn, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| intArray | Int32[] | Integer array. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| isVertical | Boolean | Specifies to import data vertically or horizontally. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodImportArrayWithInt32Int32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare Int32 array data
int[] data = new int[] { 1, 2, 3, 4, 5 };
try
{
// Call ImportArray with parameters: (Int32[], firstRow=2, firstColumn=1, isVertical=true)
worksheet.Cells.ImportArray(data, 2, 1, true);
Console.WriteLine("Imported array vertically starting from cell B3:");
for (int i = 0; i < data.Length; i++)
{
Console.WriteLine($"Cell B{3 + i}: {worksheet.Cells[2 + i, 1].Value}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
}
// Save the result
workbook.Save("CellsMethodImportArrayWithInt32Int32Int32BooleanDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportArray(double[], int, int) {#importarray}
```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn)
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportArray(double[], int, int, bool) {#importarray_1}
Imports an array of double into a worksheet.
```csharp
public void ImportArray(double[] doubleArray, int firstRow, int firstColumn, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| doubleArray | Double[] | Double array. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| isVertical | Boolean | Specifies to import data vertically or horizontally. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodImportArrayWithDoubleInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare sample double array data
double[] dataArray = new double[] { 1.23, 4.56, 7.89, 10.11, 12.13 };
const int targetRow = 2;    // 0-based row index (3rd row)
const int targetColumn = 1; // 0-based column index (2nd column)
const bool isVertical = true;
try
{
// Get cells collection and call ImportArray
Cells cells = worksheet.Cells;
cells.ImportArray(dataArray, targetRow, targetColumn, isVertical);
Console.WriteLine($"Imported {dataArray.Length} double values starting at row {targetRow + 1}, column {targetColumn + 1}");
Console.WriteLine($"Data orientation: {(isVertical ? "Vertical" : "Horizontal")}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ImportArray method: {ex.Message}");
}
// Save the result
workbook.Save("CellsImportArrayDoubleVerticalDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
