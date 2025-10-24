##WorksheetCollection.RemoveAt
WorksheetCollection method. Removes the element at a specified name
## RemoveAt(string) {#removeat_2}
Removes the element at a specified name.
```csharp
public void RemoveAt(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | The name of the element to remove. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodRemoveAtWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Add some worksheets
wb.Worksheets.Add("Sheet2");
wb.Worksheets.Add("Sheet3");
// Add a named range (fixed)
int nameIndex = wb.Worksheets.Names.Add("testname");
wb.Worksheets.Names[nameIndex].RefersTo = "=[Book1.xlsx]Sheet1!$A1";
// Demonstrate RemoveAt with string parameter
Console.WriteLine($"Before removal - Worksheet count: {wb.Worksheets.Count}");
wb.Worksheets.RemoveAt("Sheet1");
Console.WriteLine($"After removal - Worksheet count: {wb.Worksheets.Count}");
// Save the workbook
using (MemoryStream ms = new MemoryStream())
{
wb.Save(ms, SaveFormat.Xlsx);
}
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## RemoveAt(int) {#removeat}
Removes the element at a specified index.
```csharp
public void RemoveAt(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index value of the element to remove. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodRemoveAtWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Add some worksheets
wb.Worksheets.Add("Sheet1");
wb.Worksheets.Add("Sheet2");
wb.Worksheets.Add("Sheet3");
// Display original worksheet count
Console.WriteLine($"Original worksheet count: {wb.Worksheets.Count}");
// Remove worksheet at index 1 (second worksheet)
wb.Worksheets.RemoveAt(1);
// Display updated worksheet count
Console.WriteLine($"After removal, worksheet count: {wb.Worksheets.Count}");
// Save the workbook
wb.Save("output.xlsx");
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
