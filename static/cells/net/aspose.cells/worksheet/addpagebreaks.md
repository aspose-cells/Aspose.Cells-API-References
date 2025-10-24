##Worksheet.AddPageBreaks
Worksheet method. Adds page break
## Worksheet.AddPageBreaks method
Adds page break.
```csharp
public void AddPageBreaks(string cellName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | String |  |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetMethodAddPageBreaksWithStringDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add horizontal page break at row 1 (B2)
worksheet.AddPageBreaks("B2");
// Add horizontal page break at row 9 (B10)
worksheet.AddPageBreaks("B10");
// Verify the first page break was added at row 1
Console.WriteLine("First page break row: " + worksheet.HorizontalPageBreaks[0].Row);
}
}
}
```
### See Also
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
