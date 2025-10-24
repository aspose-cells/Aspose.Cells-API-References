##Cells.ImportObjectArray
Cells method. Imports an array of data into a worksheet
## ImportObjectArray(object[], int, int, bool) {#importobjectarray}
Imports an array of data into a worksheet.
```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical)
```
| Parameter | Type | Description |
| --- | --- | --- |
| objArray | Object[] | Data array. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| isVertical | Boolean | Specifies to import data vertically or horizontally. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare an object array with sample data
object[] dataArray = new object[] { "Product", "Price", "Stock", "Discontinued", 150.5, 75, false };
try
{
// Import the object array into the worksheet starting at cell B3 (row 2, column 1), horizontally
worksheet.Cells.ImportObjectArray(dataArray, 2, 1, false);
Console.WriteLine("Object array imported successfully to cells B3:F3");
}
catch (Exception ex)
{
Console.WriteLine($"Error importing data: {ex.Message}");
}
// Save the workbook to demonstrate the output
workbook.Save("CellsMethodImportObjectArrayWithObjectInt32Int32BooleanDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## ImportObjectArray(object[], int, int, bool, int) {#importobjectarray_1}
Imports an array of data into a worksheet.
```csharp
public void ImportObjectArray(object[] objArray, int firstRow, int firstColumn, bool isVertical,
int skip)
```
| Parameter | Type | Description |
| --- | --- | --- |
| objArray | Object[] | Data array. |
| firstRow | Int32 | The row number of the first cell to import in. |
| firstColumn | Int32 | The column number of the first cell to import in. |
| isVertical | Boolean | Specifies to import data vertically or horizontally. |
| skip | Int32 | Skipped number of rows or columns. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare data for ImportObjectArray parameters: (Object[], Int32, Int32, Boolean, Int32)
object[] data = new object[]
{
"Name",
"Age",
"Date",
"John Doe",
30,
new DateTime(2023, 10, 15),
"Jane Smith",
28,
new DateTime(2023, 10, 16)
};
try
{
// Call ImportObjectArray with parameters: (data array, start row 0, start column 0, horizontal import, skip 1 column between entries)
worksheet.Cells.ImportObjectArray(data, 0, 0, false, 1);
Console.WriteLine("Imported object array with parameters (Object[], 0, 0, false, 1) successfully.");
// Demonstrate effect: Data will be placed in cells A1, C1, E1, A2, C2, E2, etc. with skipped columns
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ImportObjectArray: {ex.Message}");
}
// Save the result
workbook.Save("CellsMethodImportObjectArrayWithObjectArrayInt32Int32BooleanInt32Demo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
