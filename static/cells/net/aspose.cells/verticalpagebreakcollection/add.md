##VerticalPageBreakCollection.Add
VerticalPageBreakCollection method. Adds a vertical page break to the collection
## Add(int, int, int) {#add_2}
Adds a vertical page break to the collection.
```csharp
public int Add(int startRow, int endRow, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index, zero based. |
| endRow | Int32 | End row index, zero based. |
| column | Int32 | Column index, zero based. |
### Return Value
[`VerticalPageBreak`](../../verticalpagebreak/) object index.
### Remarks
This method is used to add a vertical pagebreak within a print area.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VerticalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
// Demonstrate Add with (Int32, Int32, Int32) parameters
verticalPageBreaks.Add(0, 10, 2); // From row 0 to 10 at column 2
// Additional examples for context
verticalPageBreaks.Add(4); // At column 4
verticalPageBreaks.Add(5, 3); // At row 5, column 3
Console.WriteLine("Vertical Page Breaks:");
for (int i = 0; i < verticalPageBreaks.Count; i++)
{
VerticalPageBreak vpb = verticalPageBreaks[i];
Console.WriteLine($"{i}: StartRow={vpb.StartRow}, EndRow={vpb.EndRow}, Column={vpb.Column}");
}
workbook.Save("VerticalPageBreakDemo.xlsx");
}
}
}
```
### See Also
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(int) {#add}
Adds a vertical page break to the collection.
```csharp
public int Add(int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Cell column index, zero based. |
### Return Value
[`VerticalPageBreak`](../../verticalpagebreak/) object index.
### Remarks
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VerticalPageBreakCollectionMethodAddWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
VerticalPageBreakCollection verticalPageBreaks = worksheet.VerticalPageBreaks;
// Demonstrate Add method with Int32 parameter
verticalPageBreaks.Add(4); // Add vertical page break at column 4
// Print the added page break details
VerticalPageBreak vpb = verticalPageBreaks[0];
Console.WriteLine($"Vertical Page Break: StartRow = {vpb.StartRow}, EndRow = {vpb.EndRow}, Column = {vpb.Column}");
workbook.Save("VerticalPageBreakCollectionExample.xlsx");
}
}
}
```
### See Also
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(int, int) {#add_1}
Adds a vertical page break to the collection.
```csharp
public int Add(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Cell row index, zero based. |
| column | Int32 | Cell column index, zero based. |
### Return Value
[`VerticalPageBreak`](../../verticalpagebreak/) object index.
### Remarks
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VerticalPageBreakCollectionMethodAddWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Get the vertical page breaks collection
VerticalPageBreakCollection vPageBreaks = worksheet.VerticalPageBreaks;
// Add vertical page breaks at different column positions
vPageBreaks.Add(0, 5);  // Add page break after column 5
vPageBreaks.Add(0, 10); // Add page break after column 10
vPageBreaks.Add(0, 15); // Add page break after column 15
// Add some sample data to visualize the page breaks
for (int i = 0; i < 20; i++)
{
worksheet.Cells[0, i].PutValue($"Column {i + 1}");
}
// Save the workbook
workbook.Save("VerticalPageBreaksDemo.xlsx");
}
}
}
```
### See Also
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(string) {#add_3}
Adds a vertical page break to the collection.
```csharp
public int Add(string cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
### Return Value
[`VerticalPageBreak`](../../verticalpagebreak/) object index.
### Remarks
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class VerticalPageBreakCollectionMethodAddWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.VerticalPageBreaks.Add("G5");
VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
Console.WriteLine("Start Row: " + vpb.StartRow);
Console.WriteLine("End Row: " + vpb.EndRow);
Console.WriteLine("Column: " + vpb.Column);
}
}
}
```
### See Also
* class [VerticalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
