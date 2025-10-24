##Worksheet.Hyperlinks
Worksheet property. Gets the HyperlinkCollection collection
## Worksheet.Hyperlinks property
Gets the [`HyperlinkCollection`](../../hyperlinkcollection/) collection.
```csharp
public HyperlinkCollection Hyperlinks { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyHyperlinksDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add a hyperlink to the worksheet
worksheet.Hyperlinks.Add(0, 0, 1, 1, @"https://www.aspose.com");
// Save the workbook
workbook.Save("HyperlinksDemo.xlsx");
// Load the saved workbook to verify the hyperlink
Workbook loadedWorkbook = new Workbook("HyperlinksDemo.xlsx");
Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
// Display the hyperlink address
Console.WriteLine("Hyperlink Address: " + loadedWorksheet.Hyperlinks[0].Address);
}
}
}
```
### See Also
* class [HyperlinkCollection](../../hyperlinkcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
