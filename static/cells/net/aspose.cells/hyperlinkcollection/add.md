##HyperlinkCollection.Add
HyperlinkCollection method. Adds a hyperlink to a specified cell or a range of cells
## Add(int, int, int, int, string) {#add}
Adds a hyperlink to a specified cell or a range of cells.
```csharp
public int Add(int firstRow, int firstColumn, int totalRows, int totalColumns, string address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | Int32 | First row of the hyperlink range. |
| firstColumn | Int32 | First column of the hyperlink range. |
| totalRows | Int32 | Number of rows in this hyperlink range. |
| totalColumns | Int32 | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |
### Return Value
[`Hyperlink`](../../hyperlink/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkCollectionMethodAddWithInt32Int32Int32Int32StringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add hyperlink using row/column coordinates and dimensions
worksheet.Hyperlinks.Add(0, 0, 1, 1, "http://www.aspose.com");
worksheet.Hyperlinks.Add(1, 0, 1, 1, "c:\\book1.xls");
workbook.Save("HyperlinkDemo.xlsx");
}
}
}
```
### See Also
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(string, int, int, string) {#add_1}
Adds a hyperlink to a specified cell or a range of cells.
```csharp
public int Add(string cellName, int totalRows, int totalColumns, string address)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
| totalRows | Int32 | Number of rows in this hyperlink range. |
| totalColumns | Int32 | Number of columns of this hyperlink range. |
| address | String | Address of the hyperlink. |
### Return Value
[`Hyperlink`](../../hyperlink/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkCollectionMethodAddWithStringInt32Int32StringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
// Add hyperlink to cell A1 with address "www.aspose.com"
hyperlinks.Add("A1", 1, 1, "www.aspose.com");
// Display the hyperlink address
Console.WriteLine("Hyperlink Address: " + worksheet.Cells["A1"].StringValue);
// Change the display text
worksheet.Cells["A1"].PutValue("Click Here");
Console.WriteLine("Display Text: " + hyperlinks[0].TextToDisplay);
workbook.Save("HyperlinkExample.xlsx");
}
}
}
```
### See Also
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(string, string, string, string, string) {#add_2}
Adds a hyperlink to a specified cell or a range of cells.
```csharp
public int Add(string startCellName, string endCellName, string address, string textToDisplay,
string screenTip)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | String | The top-left cell of the range. |
| endCellName | String | The bottom-right cell of the range. |
| address | String | Address of the hyperlink. |
| textToDisplay | String | The text to be displayed for the specified hyperlink. |
| screenTip | String | The screenTip text for the specified hyperlink. |
### Return Value
[`Hyperlink`](../../hyperlink/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkCollectionMethodAddWithStringStringStringStringStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
// Demonstrate Add method with (String, String, String, String, String) parameters
hyperlinks.Add("D1", "D2", "http://www.display.com", "Click Here", "Go to Display");
workbook.Save("HyperlinkCollectionExample.xlsx");
}
}
}
```
### See Also
* class [HyperlinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
