##SheetSet.SheetSet
SheetSet constructor. Creates a sheet set based on exact sheet indexes
## SheetSet(params int[]) {#constructor}
Creates a sheet set based on exact sheet indexes.
```csharp
public SheetSet(params int[] sheetIndexes)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndexes | Int32[] | zero based sheet indexes. |
### Remarks
If a sheet is encountered that is not in the workbook, an exception will be thrown during rendering.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class SheetSetMethodCtorWithInt32ArrayDemo
{
public static void Run()
{
// Create a new workbook with 3 worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Add identification text to each sheet
workbook.Worksheets[0].Cells["A1"].PutValue("This is Sheet 1");
workbook.Worksheets[1].Cells["A1"].PutValue("This is Sheet 2");
workbook.Worksheets[2].Cells["A1"].PutValue("This is Sheet 3");
try
{
// Create SheetSet with specific sheet indexes (0 and 2)
SheetSet sheetSet = new SheetSet(new int[] { 0, 2 });
// Create PDF save options with our sheet set
PdfSaveOptions options = new PdfSaveOptions();
options.SheetSet = sheetSet;
// Save the workbook with selected sheets
workbook.Save("SheetSetDemo.pdf", options);
Console.WriteLine("Created PDF containing Sheet 1 and Sheet 3");
}
catch (ArgumentOutOfRangeException ex)
{
Console.WriteLine($"Invalid sheet index specified: {ex.Message}");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## SheetSet(params string[]) {#constructor_1}
Creates a sheet set based on exact sheet names.
```csharp
public SheetSet(params string[] sheetNames)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetNames | String[] | sheet names. |
### Remarks
If a sheet is encountered that is not in the workbook, an exception will be thrown during rendering.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class SheetSetMethodCtorWithStringArrayDemo
{
public static void Run()
{
// Create a new workbook and add sheets
Workbook workbook = new Workbook();
workbook.Worksheets[0].Name = "First";
workbook.Worksheets.Add("Second");
workbook.Worksheets.Add("Third");
workbook.Worksheets["First"].Cells["A1"].PutValue("This is Sheet 1");
workbook.Worksheets["Second"].Cells["A1"].PutValue("This is Sheet 2");
workbook.Worksheets["Third"].Cells["A1"].PutValue("This is Sheet 3");
// Prepare sheet names for SheetSet
string[] selectedSheets = { "First", "Third" };
try
{
// Create SheetSet with string array parameter
SheetSet sheetSet = new SheetSet(selectedSheets);
// Configure PDF save options with created SheetSet
PdfSaveOptions pdfOptions = new PdfSaveOptions();
pdfOptions.SheetSet = sheetSet;
// Save workbook to PDF with specified sheets
workbook.Save("SheetSetOutput.pdf", pdfOptions);
Console.WriteLine("Created PDF with sheets: " + string.Join(", ", selectedSheets));
}
catch (Exception ex)
{
Console.WriteLine($"Error creating SheetSet: {ex.Message}");
}
}
}
}
```
### See Also
* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
