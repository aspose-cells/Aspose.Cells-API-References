##WorksheetCollection.AddCopy
WorksheetCollection method. Adds a worksheet to the collection and copies data from an existed worksheet
## AddCopy(string) {#addcopy_1}
Adds a worksheet to the collection and copies data from an existed worksheet.
```csharp
public int AddCopy(string sheetName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Name of source worksheet. |
### Return Value
[`Worksheet`](../../worksheet/) object index.
### Exceptions
| exception | condition |
| --- | --- |
| [CellsException](../../cellsexception/) | Specifies an invalid worksheet name. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodAddCopyWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet named "Original" to the workbook
Worksheet originalSheet = workbook.Worksheets.Add("Original");
// Add some data to the original worksheet
originalSheet.Cells["A1"].PutValue("This is the original sheet");
// Make a copy of the "Original" worksheet
int copiedIndex = workbook.Worksheets.AddCopy("Original");
Worksheet copiedSheet = workbook.Worksheets[copiedIndex];
copiedSheet.Name = "CopiedSheet";
// Modify the copied sheet to demonstrate it's a separate copy
copiedSheet.Cells["A1"].PutValue("This is the copied sheet");
// Save the workbook
workbook.Save("WorksheetCopyDemo.xlsx");
Console.WriteLine("Worksheet copied successfully. Output file: WorksheetCopyDemo.xlsx");
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AddCopy(int) {#addcopy}
Adds a worksheet to the collection and copies data from an existed worksheet.
```csharp
public int AddCopy(int sheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Int32 | Index of source worksheet. |
### Return Value
[`Worksheet`](../../worksheet/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodAddCopyWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet and add some data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Original Worksheet");
// Add a copy of the first worksheet
workbook.Worksheets.AddCopy(0);
// Verify the copy was created
Worksheet copiedWorksheet = workbook.Worksheets[1];
copiedWorksheet.Cells["A1"].PutValue("Copied Worksheet");
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AddCopy(Worksheet[], string[]) {#addcopy_2}
Copy a group of worksheets.
```csharp
public void AddCopy(Worksheet[] source, string[] destSheetNames)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | Worksheet[] | The source worksheets. |
| destSheetNames | String[] | The names of the copied sheets. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class WorksheetCollectionMethodAddCopyWithWorksheetStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some sample worksheets
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Populate some data in the worksheets
workbook.Worksheets["Sheet2"].Cells["A1"].PutValue("Original Sheet1 Data");
workbook.Worksheets["Sheet3"].Cells["A1"].PutValue("Original Sheet2 Data");
// Prepare source worksheets array
Worksheet[] sourceSheets = new Worksheet[]
{
workbook.Worksheets["Sheet2"],
workbook.Worksheets["Sheet3"]
};
// Prepare destination sheet names array
string[] destSheetNames = new string[]
{
"CopyOfSheet2",
"CopyOfSheet3"
};
try
{
// Call the AddCopy method with (Worksheet[], String[]) parameters
workbook.Worksheets.AddCopy(sourceSheets, destSheetNames);
Console.WriteLine("AddCopy method executed successfully with parameters (Worksheet[], String[])");
// Verify the copies were created
Console.WriteLine($"Total worksheets after copy: {workbook.Worksheets.Count}");
foreach (Worksheet sheet in workbook.Worksheets)
{
Console.WriteLine($"Worksheet name: {sheet.Name}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing AddCopy method: {ex.Message}");
}
// Save the result
workbook.Save("WorksheetCollectionMethodAddCopyDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
