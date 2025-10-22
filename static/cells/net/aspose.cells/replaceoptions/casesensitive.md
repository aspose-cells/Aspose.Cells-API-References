##ReplaceOptions.CaseSensitive
ReplaceOptions property. Indicates if the searched string is case sensitive
## ReplaceOptions.CaseSensitive property
Indicates if the searched string is case sensitive.
```csharp
public bool CaseSensitive { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReplaceOptionsPropertyCaseSensitiveDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("apple");
worksheet.Cells["A3"].PutValue("Apple");
worksheet.Cells["A4"].PutValue("APPLE");
// Create replace options with CaseSensitive = false
ReplaceOptions options = new ReplaceOptions();
options.CaseSensitive = false;
// Replace all case variations of "apple" with "orange"
workbook.Replace("apple", "orange", options);
// Output results
Console.WriteLine("After replacement (CaseSensitive = false):");
for (int i = 1; i <= 4; i++)
{
Console.WriteLine(worksheet.Cells["A" + i].StringValue);
}
// Reset data
worksheet.Cells["A2"].PutValue("apple");
worksheet.Cells["A3"].PutValue("Apple");
worksheet.Cells["A4"].PutValue("APPLE");
// Change to CaseSensitive = true
options.CaseSensitive = true;
workbook.Replace("apple", "orange", options);
// Output results
Console.WriteLine("\nAfter replacement (CaseSensitive = true):");
for (int i = 1; i <= 4; i++)
{
Console.WriteLine(worksheet.Cells["A" + i].StringValue);
}
}
}
}
```
### See Also
* class [ReplaceOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
