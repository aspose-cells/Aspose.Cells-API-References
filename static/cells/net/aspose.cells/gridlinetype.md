##Enum GridlineType
Aspose.Cells.GridlineType enum. Enumerates grid line Type
## GridlineType enumeration
Enumerates grid line Type.
```csharp
public enum GridlineType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Dotted | `0` | Represents dotted line. |
| Hair | `1` | Represents hair line. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassGridlineTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Create save options and set gridline type
DocxSaveOptions saveOptions = new DocxSaveOptions();
saveOptions.GridlineType = GridlineType.Dotted;
// Add some sample data to see gridlines
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["B2"].PutValue(123);
worksheet.Cells["C3"].PutValue(DateTime.Now);
// Save the workbook with the save options
workbook.Save("GridlineTypeDemo.docx", saveOptions);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
