##Cells.InsertColumn
Cells method. Inserts a new column into the worksheet
## InsertColumn(int, bool) {#insertcolumn_1}
Inserts a new column into the worksheet.
```csharp
public void InsertColumn(int columnIndex, bool updateReference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| updateReference | Boolean | Indicates if references in other worksheets will be updated. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertColumnWithInt32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Populate some sample data in column 0
Cells cells = sheet.Cells;
for (int i = 0; i < 5; i++)
{
cells[i, 0].PutValue($"Original {i}");
}
// Insert a new column at index 1 and shift columns right
cells.InsertColumn(1, true);
// Copy data from column 0 to the new column 1
cells.CopyColumn(cells, 0, 1);
// Save the workbook
workbook.Save("InsertColumnDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## InsertColumn(int) {#insertcolumn}
Inserts a new column into the worksheet.
```csharp
public void InsertColumn(int columnIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertColumnWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Get the cells collection
Cells cells = sheet.Cells;
// Insert data into cells for demonstration
cells["A1"].PutValue("Column A");
cells["B1"].PutValue("Column B");
cells["C1"].PutValue("Column C");
// Insert a new column at index 1 (will become the new column B)
cells.InsertColumn(1);
// Verify by inserting data into the new column
cells["B1"].PutValue("New Column");
// Save the workbook
workbook.Save("InsertColumnDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
