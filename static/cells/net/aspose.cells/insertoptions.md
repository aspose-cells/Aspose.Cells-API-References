##Class InsertOptions
Aspose.Cells.InsertOptions class. Represents the options of inserting
## InsertOptions class
Represents the options of inserting.
```csharp
public class InsertOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [InsertOptions](insertoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [CopyFormatType](../../aspose.cells/insertoptions/copyformattype/) { get; set; } |  |
| [FormulaChangeMonitor](../../aspose.cells/insertoptions/formulachangemonitor/) { get; set; } | Gets/sets the monitor for tracking changes caused by the insertion. |
| [UpdateReference](../../aspose.cells/insertoptions/updatereference/) { get; set; } | Indicates if references in other worksheets will be updated. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class InsertOptionsDemo
{
public static void InsertOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of InsertOptions
InsertOptions insertOptions = new InsertOptions
{
CopyFormatType = CopyFormatType.SameAsAbove,
UpdateReference = true
};
// Define the cell area where rows will be inserted
CellArea cellArea = new CellArea { StartRow = 0, EndRow = 10, StartColumn = 0, EndColumn = 10 };
// Insert rows with the specified options
worksheet.Cells.InsertRows(5, 3, insertOptions);
// Save the workbook
workbook.Save("InsertOptionsExample.xlsx");
workbook.Save("InsertOptionsExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
