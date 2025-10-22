##ExternalLinkCollection.Item
ExternalLinkCollection property. Gets the ExternalLink element at the specified index
## ExternalLinkCollection indexer
Gets the [`ExternalLink`](../../externallink/) element at the specified index.
```csharp
public ExternalLink this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The zero based index of the element. |
### Return Value
The element at the specified index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook with sample external links
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some external links
worksheet.Cells["A1"].Formula = "='C:\\Temp\\External1.xlsx'!A1";
worksheet.Cells["A2"].Formula = "='C:\\Temp\\External2.xlsx'!B2";
// Access external links using Item property
for (int i = 0; i < workbook.Worksheets.ExternalLinks.Count; i++)
{
ExternalLink link = workbook.Worksheets.ExternalLinks[i];
Console.WriteLine($"External Link {i + 1}:");
Console.WriteLine($"- DataSource: {link.DataSource}");
Console.WriteLine($"- OriginalDataSource: {link.OriginalDataSource}");
}
}
}
}
```
### See Also
* class [ExternalLink](../../externallink/)
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
