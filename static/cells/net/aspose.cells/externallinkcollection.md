##Class ExternalLinkCollection
Aspose.Cells.ExternalLinkCollection class. Represents external links collection in a workbook
## ExternalLinkCollection class
Represents external links collection in a workbook.
```csharp
public class ExternalLinkCollection : IEnumerable
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells/externallinkcollection/count/) { get; } | Gets the number of elements actually contained in the collection. |
| [Item](../../aspose.cells/externallinkcollection/item/) { get; } | Gets the [`ExternalLink`](../externallink/) element at the specified index. |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/externallinkcollection/add/#add_1)(string, string[]) | Adds an external link. |
| [Add](../../aspose.cells/externallinkcollection/add/#add)(DirectoryType, string, string[]) | Add an external link . |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear)() | Removes all external links. |
| [Clear](../../aspose.cells/externallinkcollection/clear/#clear_1)(bool) | Removes all external links. |
| [GetEnumerator](../../aspose.cells/externallinkcollection/getenumerator/)() | Get an enumerator that iterates through this collection. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat)(int) | Removes the specified external link from the workbook. |
| [RemoveAt](../../aspose.cells/externallinkcollection/removeat/#removeat_1)(int, bool) | Removes the specified external link from the workbook. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ExternalLinkCollectionDemo
{
public static void ExternalLinkCollectionExample()
{
// Open a file with external links
Workbook workbook = new Workbook("ExternalLinkCollectionExample_original.xlsx");
// Get the external links collection
ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
// Display the count of external links
Console.WriteLine("Number of external links: " + externalLinks.Count);
// Iterate through the external links and display their data sources
for (int i = 0; i < externalLinks.Count; i++)
{
ExternalLink link = externalLinks[i];
Console.WriteLine("External Link " + i + " Data Source: " + link.DataSource);
}
// Add a new external link
int newLinkIndex = externalLinks.Add("newLink.xls", new[] { "Sheet1" });
Console.WriteLine("Added new external link at index: " + newLinkIndex);
// Change the data source of the first external link
if (externalLinks.Count > 0)
{
externalLinks[0].DataSource = "d:\\link.xlsx";
Console.WriteLine("Updated data source of the first external link.");
}
// Save the workbook
workbook.Save("ExternalLinkCollectionExample.xlsx");
// Clear all external links
externalLinks.Clear();
Console.WriteLine("Cleared all external links.");
// Save the workbook after clearing external links
workbook.Save("ExternalLinkCollectionExample2.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
