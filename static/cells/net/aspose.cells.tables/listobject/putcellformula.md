##ListObject.PutCellFormula
ListObject method. Put the formula to the cell in the table
## PutCellFormula(int, int, string) {#putcellformula}
Put the formula to the cell in the table.
```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| formula | String | The formula of the cell. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectMethodPutCellFormulaWithInt32Int32StringDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data to create a table
sheet.Cells["A1"].PutValue("ID");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["C1"].PutValue("Formula");
sheet.Cells["A2"].PutValue(1);
sheet.Cells["B2"].PutValue(10);
sheet.Cells["A3"].PutValue(2);
sheet.Cells["B3"].PutValue(20);
// Create a list object (table)
int index = sheet.ListObjects.Add("A1", "C3", true);
ListObject table = sheet.ListObjects[index];
// Add a new row and set values/formula
table.PutCellValue(4, 0, 3); // Row 4, Column 0 (ID)
table.PutCellValue(4, 1, 30); // Row 4, Column 1 (Value)
table.PutCellFormula(4, 2, "=B3*2"); // Row 4, Column 2 (Formula)
// Save the workbook
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
## PutCellFormula(int, int, string, bool) {#putcellformula_1}
Put the formula to the cell in the table.
```csharp
public void PutCellFormula(int rowOffset, int columnOffset, string formula, bool isTotalsRowFormula)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | The row offset in the table. |
| columnOffset | Int32 | The column offset in the table. |
| formula | String | The formula of the cell. |
| isTotalsRowFormula | Boolean |  |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class ListObjectMethodPutCellFormulaWithInt32Int32StringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a list object
worksheet.Cells["A1"].PutValue("Column1");
worksheet.Cells["A2"].PutValue(10);
worksheet.Cells["A3"].PutValue(20);
// Create list object
int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
ListObject listObject = worksheet.ListObjects[index];
// Demonstrate PutCellFormula
listObject.PutCellFormula(3, 0, "=SUM(A2:A3)", true);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
