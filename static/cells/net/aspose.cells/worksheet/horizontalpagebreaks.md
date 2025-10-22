##Worksheet.HorizontalPageBreaks
Worksheet property. Gets the HorizontalPageBreakCollection collection
## Worksheet.HorizontalPageBreaks property
Gets the [`HorizontalPageBreakCollection`](../../horizontalpagebreakcollection/) collection.
```csharp
public HorizontalPageBreakCollection HorizontalPageBreaks { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyHorizontalPageBreaksDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add horizontal page breaks in different ways
worksheet.HorizontalPageBreaks.Add(5);
worksheet.HorizontalPageBreaks.Add(10, 1, 5);
worksheet.HorizontalPageBreaks.Add(15, 2);
worksheet.HorizontalPageBreaks.Add("G5");
// Remove the first page break
worksheet.HorizontalPageBreaks.RemoveAt(0);
// Save outputs
workbook.Save("HorizontalPageBreaksDemo.xlsx");
workbook.Save("HorizontalPageBreaksDemo.pdf");
}
}
}
```
### See Also
* class [HorizontalPageBreakCollection](../../horizontalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
