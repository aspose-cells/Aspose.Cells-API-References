##ExternalLinkCollection.GetEnumerator
ExternalLinkCollection method. Get an enumerator that iterates through this collection
## ExternalLinkCollection.GetEnumerator method
Get an enumerator that iterates through this collection.
```csharp
public IEnumerator GetEnumerator()
```
### Examples
```csharp
using System;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ExternalLinkCollectionMethodGetEnumeratorDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add some external links using the correct Add method signature
workbook.Worksheets.ExternalLinks.Add("externallink1.xlam", new string[] { "Sheet1!A1" });
workbook.Worksheets.ExternalLinks.Add("externallink2.xlam", new string[] { "Sheet1!A1" });
workbook.Worksheets.ExternalLinks.Add("externallink3.xlam", new string[] { "Sheet1!A1" });
workbook.Worksheets.ExternalLinks.Add("externallink4.xlam", new string[] { "Sheet1!A1" });
// Get the ExternalLinkCollection
ExternalLinkCollection externalLinks = workbook.Worksheets.ExternalLinks;
// Demonstrate GetEnumerator usage
Console.WriteLine("Enumerating external links:");
IEnumerator enumerator = externalLinks.GetEnumerator();
int count = 0;
while (enumerator.MoveNext())
{
ExternalLink link = (ExternalLink)enumerator.Current;
Console.WriteLine($"{++count}. {link.DataSource}");
}
// Add formulas referencing these external links
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 4; i++)
{
worksheet.Cells[i, 0].Formula = $"=externallink{i+1}.xlam!customfunc()";
}
Console.WriteLine("\nFormulas referencing external links:");
for (int i = 0; i < 4; i++)
{
Console.WriteLine($"Cell A{i+1}: {worksheet.Cells[i, 0].Formula}");
}
}
}
}
```
### See Also
* class [ExternalLinkCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
