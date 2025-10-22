##Cells.Item
Cells property. Gets the Cell element at the specified cell row index and column index
## Cells indexer (1 of 2)
Gets the [`Cell`](../../cell/) element at the specified cell row index and column index.
```csharp
public Cell this[int row, int column] { get; }
```
| Parameter | Description |
| --- | --- |
| row | Row index. |
| column | Column index. |
### Return Value
The [`Cell`](../../cell/) object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Using Item property to access and modify cells
cells[0, 0].PutValue("Hello");
cells[1, 0].PutValue("World");
// Using Style property through Cells
Style style1 = cells[0, 0].GetStyle();
style1.Font.IsBold = true;
cells[0, 0].SetStyle(style1);
Style style2 = cells[1, 0].GetStyle();
style2.Font.Color = System.Drawing.Color.Red;
cells[1, 0].SetStyle(style2);
// Save the workbook
workbook.Save("CellsPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Cells indexer (2 of 2)
Gets the [`Cell`](../../cell/) element at the specified cell name.
```csharp
public Cell this[string cellName] { get; }
```
| Parameter | Description |
| --- | --- |
| cellName | Cell name,including its column letter and row number, for example A5. |
### Return Value
A [`Cell`](../../cell/) object
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsPropertyItemDemo1
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access the cells collection
Cells cells = worksheet.Cells;
// Set values using Item property
cells["A1"].PutValue("Name");
cells["B1"].PutValue("Age");
// Set values in a range using Item property
cells["A2"].PutValue("John");
cells["B2"].PutValue(30);
cells["A3"].PutValue("Alice");
cells["B3"].PutValue(25);
// Access and modify cell properties using Item
Cell cell = cells["B1"];
Style style = cell.GetStyle();
style.Font.IsBold = true;
cell.SetStyle(style);
// Save the workbook
workbook.Save("CellsPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
