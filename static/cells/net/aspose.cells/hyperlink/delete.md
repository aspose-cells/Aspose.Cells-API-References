##Hyperlink.Delete
Hyperlink method. Deletes this hyperlink
## Hyperlink.Delete method
Deletes this hyperlink
```csharp
public void Delete()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HyperlinkMethodDeleteDemo
{
public static void Run()
{
// Create a new workbook for demonstration
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some hyperlinks to demonstrate deletion
worksheet.Hyperlinks.Add("A1", 1, 1, "https://www.aspose.com");
worksheet.Hyperlinks.Add("B2", 1, 1, "https://www.example.com");
Console.WriteLine($"Hyperlinks count before deletion: {worksheet.Hyperlinks.Count}");
// Delete all hyperlinks
for (int i = worksheet.Hyperlinks.Count - 1; i >= 0; i--)
{
worksheet.Hyperlinks[i].Delete();
}
Console.WriteLine($"Hyperlinks count after deletion: {worksheet.Hyperlinks.Count}");
}
}
}
```
### See Also
* class [Hyperlink](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
