##WorksheetCollection.Item
WorksheetCollection property. Gets the Worksheet element at the specified index
## WorksheetCollection indexer (1 of 2)
Gets the [`Worksheet`](../../worksheet/) element at the specified index.
```csharp
public Worksheet this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyItemDemo1
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Using Item property to access cell
Cell cell = cells[0, 0];
cell.Formula = "=SUM(1, 2, 3)";
workbook.CalculateFormula();
Console.WriteLine("Cell value: " + cell.IntValue);
}
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## WorksheetCollection indexer (2 of 2)
Gets the [`Worksheet`](../../worksheet/) element with the specified name.
```csharp
public Worksheet this[string sheetName] { get; }
```
| Parameter | Description |
| --- | --- |
| sheetName | Worksheet name |
### Return Value
The element with the specified name.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyItemDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access worksheets using Item property by index and name
Worksheet sheet1 = workbook.Worksheets[0];
sheet1.Name = "FirstSheet";
Worksheet sheet2 = workbook.Worksheets.Add("SecondSheet");
// Access worksheet by name using Item property
Worksheet accessedSheet = workbook.Worksheets["FirstSheet"];
// Add data to demonstrate worksheet access
Cells cells = accessedSheet.Cells;
cells["A1"].PutValue("Worksheet accessed successfully!");
cells["A2"].PutValue(DateTime.Now.ToString());
// Insert a column in the second sheet
workbook.Worksheets["SecondSheet"].Cells.InsertColumn(1);
// Save the workbook
workbook.Save("WorksheetCollectionItemDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
