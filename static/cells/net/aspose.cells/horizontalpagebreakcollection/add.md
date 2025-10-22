##HorizontalPageBreakCollection.Add
HorizontalPageBreakCollection method. Adds a horizontal page break to the collection
## Add(int, int, int) {#add_2}
Adds a horizontal page break to the collection.
```csharp
public int Add(int row, int startColumn, int endColumn)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index, zero based. |
| startColumn | Int32 | Start column index, zero based. |
| endColumn | Int32 | End column index, zero based. |
### Return Value
[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.
### Remarks
This method is used to add a horizontal pagebreak within a print area.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate Add method with (Int32, Int32, Int32) parameters
worksheet.HorizontalPageBreaks.Add(10, 1, 5);
workbook.Save("HorizontalPageBreakExample.xlsx");
}
}
}
```
### See Also
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(int) {#add}
Adds a horizontal page break to the collection.
```csharp
public int Add(int row)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Cell row index, zero based. |
### Return Value
[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.
### Remarks
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HorizontalPageBreakCollectionMethodAddWithInt32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add horizontal page breaks using Int32 parameter
worksheet.HorizontalPageBreaks.Add(5);
worksheet.HorizontalPageBreaks.Add(10);
workbook.Save("HorizontalPageBreakExample.xlsx");
}
}
}
```
### See Also
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(int, int) {#add_1}
Adds a horizontal page break to the collection.
```csharp
public int Add(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Cell row index, zero based. |
| column | Int32 | Cell column index, zero based. |
### Return Value
[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.
### Remarks
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HorizontalPageBreakCollectionMethodAddWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data to create multiple rows
for (int i = 0; i < 50; i++)
{
worksheet.Cells[i, 0].Value = "Row " + (i + 1);
}
// Add horizontal page breaks at specific rows
worksheet.HorizontalPageBreaks.Add(9, 0);  // Page break after row 9
worksheet.HorizontalPageBreaks.Add(19, 0); // Page break after row 19
worksheet.HorizontalPageBreaks.Add(29, 0); // Page break after row 29
// Save the workbook
workbook.Save("HorizontalPageBreaksDemo.xlsx");
}
}
}
```
### See Also
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(string) {#add_3}
Adds a horizontal page break to the collection.
```csharp
public int Add(string cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String | Cell name. |
### Return Value
[`HorizontalPageBreak`](../../horizontalpagebreak/) object index.
### Remarks
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HorizontalPageBreakCollectionMethodAddWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add horizontal page break at row 4 (D5 is row 4 in zero-based index)
worksheet.HorizontalPageBreaks.Add("D5");
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [HorizontalPageBreakCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
