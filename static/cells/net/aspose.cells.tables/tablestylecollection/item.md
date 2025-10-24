##TableStyleCollection.Item
TableStyleCollection property. Gets the table style by the index
## TableStyleCollection indexer (1 of 2)
Gets the table style by the index.
```csharp
public TableStyle this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The position of the table style in the list. |
### Return Value
The table style object.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TableStyleCollectionPropertyItemDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Style firstColumnStyle = workbook.CreateStyle();
firstColumnStyle.Pattern = BackgroundType.Solid;
firstColumnStyle.BackgroundColor = System.Drawing.Color.LightBlue;
Style lastColumnStyle = workbook.CreateStyle();
lastColumnStyle.Font.IsBold = true;
lastColumnStyle.ForegroundColor = System.Drawing.Color.LightGreen;
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
int index = tableStyles.AddTableStyle("CustomStyle1");
TableStyle tableStyle = tableStyles[index];
TableStyleElementCollection elements = tableStyle.TableStyleElements;
elements.Add(TableStyleElementType.FirstColumn);
elements[0].SetElementStyle(firstColumnStyle);
elements.Add(TableStyleElementType.LastColumn);
elements[1].SetElementStyle(lastColumnStyle);
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].PutValue("Product");
cells["B1"].PutValue("Price");
cells["A2"].PutValue("Item1");
cells["B2"].PutValue(100);
cells["A3"].PutValue("Item2");
cells["B3"].PutValue(200);
int tableIndex = workbook.Worksheets[0].ListObjects.Add(0, 0, 3, 1, true);
ListObject table = workbook.Worksheets[0].ListObjects[tableIndex];
table.TableStyleName = "CustomStyle1";
table.ShowTableStyleFirstColumn = true;
table.ShowTableStyleLastColumn = true;
workbook.Save("TableStyleDemo.xlsx");
}
}
}
```
### See Also
* class [TableStyle](../../tablestyle/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
## TableStyleCollection indexer (2 of 2)
Gets the table style by the name.
```csharp
public TableStyle this[string name] { get; }
```
| Parameter | Description |
| --- | --- |
| name | The table style name. |
### Return Value
The table style object.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class TableStyleCollectionPropertyItemDemo2
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the table style collection from the workbook
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
// Add a new custom table style
int index = tableStyles.AddTableStyle("CustomStyle1");
TableStyle customStyle = tableStyles[index];
// Set some properties of the custom style
customStyle.TableStyleElements[TableStyleElementType.FirstRowStripe].GetElementStyle().Font.IsBold = true;
// Access the style using Item property by name
TableStyle retrievedStyle = tableStyles["CustomStyle1"];
Console.WriteLine("Retrieved style name: " + retrievedStyle.Name);
// Modify the retrieved style
retrievedStyle.TableStyleElements[TableStyleElementType.FirstColumn].GetElementStyle().Font.Color = System.Drawing.Color.Red;
// Create a table to demonstrate the style
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Name");
cells["B1"].PutValue("Age");
cells["A2"].PutValue("John");
cells["B2"].PutValue(30);
cells["A3"].PutValue("Alice");
cells["B3"].PutValue(25);
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];
table.TableStyleName = "CustomStyle1";
// Save the result
workbook.Save("TableStyleCollectionPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [TableStyle](../../tablestyle/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
