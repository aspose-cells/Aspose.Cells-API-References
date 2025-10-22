##Cells.InsertColumns
Cells method. Inserts some columns into the worksheet
## InsertColumns(int, int) {#insertcolumns}
Inserts some columns into the worksheet.
```csharp
public void InsertColumns(int columnIndex, int totalColumns)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| totalColumns | Int32 | The number of columns. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertColumnsWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Insert 3 columns starting from column index 1 (second column)
worksheet.Cells.InsertColumns(1, 3);
// Add sample data to demonstrate the inserted columns
worksheet.Cells["A1"].PutValue("Original Column");
worksheet.Cells["B1"].PutValue("Inserted Column 1");
worksheet.Cells["C1"].PutValue("Inserted Column 2");
worksheet.Cells["D1"].PutValue("Inserted Column 3");
worksheet.Cells["E1"].PutValue("Original Column 2");
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## InsertColumns(int, int, bool) {#insertcolumns_2}
Inserts some columns into the worksheet.
```csharp
public void InsertColumns(int columnIndex, int totalColumns, bool updateReference)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| totalColumns | Int32 | The number of columns. |
| updateReference | Boolean | Indicates if references in other worksheets will be updated. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertColumnsWithInt32Int32BooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Insert 3 columns at column index 2 (0-based), shifting existing columns right
worksheet.Cells.InsertColumns(2, 3, true);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## InsertColumns(int, int, InsertOptions) {#insertcolumns_1}
Inserts some columns into the worksheet.
```csharp
public void InsertColumns(int columnIndex, int totalColumns, InsertOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | Int32 | Column index. |
| totalColumns | Int32 | The number of columns. |
| options | InsertOptions | The options for inserting operation. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodInsertColumnsWithInt32Int32InsertOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["C1"].PutValue("Header3");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue("Data2");
worksheet.Cells["C2"].PutValue("Data3");
// Create insert options
InsertOptions options = new InsertOptions();
options.CopyFormatType = CopyFormatType.Clear;
// Insert a column at index 1 (second column)
worksheet.Cells.InsertColumns(1, 1, options);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [InsertOptions](../../insertoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
