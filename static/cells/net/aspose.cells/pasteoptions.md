##Class PasteOptions
Aspose.Cells.PasteOptions class. Represents the paste special options
## PasteOptions class
Represents the paste special options.
```csharp
public class PasteOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [PasteOptions](pasteoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [IgnoreLinksToOriginalFile](../../aspose.cells/pasteoptions/ignorelinkstooriginalfile/) { get; set; } | Ingore links to the original file. |
| [KeepOldTables](../../aspose.cells/pasteoptions/keepoldtables/) { get; set; } | Keeps the tables in the destination range. |
| [OnlyVisibleCells](../../aspose.cells/pasteoptions/onlyvisiblecells/) { get; set; } | True means only copying visible cells. |
| [OperationType](../../aspose.cells/pasteoptions/operationtype/) { get; set; } | Gets and sets the operation type when pasting range. |
| [PasteType](../../aspose.cells/pasteoptions/pastetype/) { get; set; } | The paste special type. |
| [SkipBlanks](../../aspose.cells/pasteoptions/skipblanks/) { get; set; } | Indicates whether skips blank cells. |
| [Transpose](../../aspose.cells/pasteoptions/transpose/) { get; set; } | True to transpose rows and columns when the range is pasted. The default value is False. |
### Examples
```csharp
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PasteOptionsDemo
{
public static void PasteOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some data to the first worksheet
sheet.Cells["A1"].PutValue("Hello");
sheet.Cells["A2"].PutValue("World");
sheet.Cells["A3"].PutValue(123);
// Create another worksheet
Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
// Define the source range
Aspose.Cells.Range sourceRange = sheet.Cells.CreateRange("A1:A3");
// Define the destination range
Aspose.Cells.Range destRange = sheet2.Cells.CreateRange("B1:B3");
// Create PasteOptions object
PasteOptions pasteOptions = new PasteOptions
{
PasteType = PasteType.Values,
SkipBlanks = true,
OnlyVisibleCells = false,
Transpose = false,
OperationType = PasteOperationType.None,
IgnoreLinksToOriginalFile = true
};
// Copy the range with the specified paste options
destRange.Copy(sourceRange, pasteOptions);
// Save the workbook
workbook.Save("PasteOptionsExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
