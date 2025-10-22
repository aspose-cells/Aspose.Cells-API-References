##Cells.InsertRows
Cells method. Inserts multiple rows into the worksheet
## InsertRows(int, int, bool) {#insertrows_2}
Inserts multiple rows into the worksheet.
```csharp
public void InsertRows(int rowIndex, int totalRows, bool updateReference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
| totalRows | Int32 | Number of rows to be inserted. |
| updateReference | Boolean | Indicates if references in other worksheets will be updated. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertRowsWithInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Header");
worksheet.Cells["A2"].PutValue("Data 1");
worksheet.Cells["A3"].PutValue("Data 2");
worksheet.Cells["A4"].PutValue("Data 3");
// Insert a row at index 2 (will become the new row 3)
worksheet.Cells.InsertRows(2, 1, true);
// Add data to the inserted row
worksheet.Cells["A3"].PutValue("Inserted Data");
// Save the workbook
workbook.Save("InsertRowsDemo.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## InsertRows(int, int, InsertOptions) {#insertrows_1}
Inserts multiple rows into the worksheet.
```csharp
public void InsertRows(int rowIndex, int totalRows, InsertOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
| totalRows | Int32 | Number of rows to be inserted. |
| options | InsertOptions | Options for inserting operation. |
### Examples
```csharp
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertRowsWithInt32Int32InsertOptionsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].Value = "Row " + (i + 1);
}
InsertOptions insertOptions = new InsertOptions
{
CopyFormatType = CopyFormatType.SameAsAbove,
UpdateReference = true
};
// Insert 3 rows at row index 5 with the specified options
worksheet.Cells.InsertRows(5, 3, insertOptions);
workbook.Save("InsertRowsWithOptions.xlsx");
}
}
}
```
### See Also
* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## InsertRows(int, int) {#insertrows}
Inserts multiple rows into the worksheet.
```csharp
public void InsertRows(int rowIndex, int totalRows)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | Int32 | Row index. |
| totalRows | Int32 | Number of rows to be inserted. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertRowsWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Add some sample data
cells["A1"].PutValue("Header1");
cells["B1"].PutValue("Header2");
cells["A2"].PutValue("Data1");
cells["B2"].PutValue("Data2");
cells["A3"].PutValue("Data3");
cells["B3"].PutValue("Data4");
// Insert 2 rows at row index 2
cells.InsertRows(2, 2);
// Verify the inserted rows are empty
Console.WriteLine("Cell A2 value: " + cells[1, 0].Value); // Should be "Data1"
Console.WriteLine("Cell A3 value: " + cells[2, 0].Value); // Should be null (empty)
Console.WriteLine("Cell A4 value: " + cells[3, 0].Value); // Should be null (empty)
Console.WriteLine("Cell A5 value: " + cells[4, 0].Value); // Should be "Data3"
// Save the workbook
workbook.Save("InsertRowsDemo_out.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
