##Hyperlink.Area
Hyperlink property. Gets the range of hyperlink
## Hyperlink.Area property
Gets the range of hyperlink.
```csharp
public CellArea Area { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkPropertyAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Main Menu");
worksheet.Cells["A3"].PutValue("Chapter 1");
worksheet.Cells["A4"].PutValue("Chapter 2");
// Add hyperlinks
int hyperlinkIndex1 = worksheet.Hyperlinks.Add("A3", 1, 1, "Sheet2!A1");
int hyperlinkIndex2 = worksheet.Hyperlinks.Add("A4", 1, 1, "Sheet3!A1");
// Access hyperlinks and demonstrate Area property usage
HyperlinkCollection hyperlinks = worksheet.Hyperlinks;
string chapter2Address = "";
foreach (Hyperlink link in hyperlinks)
{
// Check if hyperlink is in cell A4 using Area property
if (link.Area.StartRow == 3 && link.Area.StartColumn == 0)
{
chapter2Address = link.Address;
break;
}
}
Console.WriteLine("Chapter 2 hyperlink address: " + chapter2Address);
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
