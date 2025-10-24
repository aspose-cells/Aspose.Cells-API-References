##FindOptions.CaseSensitive
FindOptions property. Indicates if the searched string is case sensitive
## FindOptions.CaseSensitive property
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
public class FindOptionsPropertyCaseSensitiveDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data
worksheet.Cells["A1"].PutValue("ABC");
worksheet.Cells["A2"].PutValue("abc");
worksheet.Cells["A3"].PutValue("BcD");
FindOptions options = new FindOptions();
options.CaseSensitive = true;
// Search for "bc" with case sensitivity
Cell cell = worksheet.Cells.Find("bc", null, options);
Console.WriteLine(cell == null ? "Not found (case sensitive)" : $"Found at: {cell.Name}");
options.CaseSensitive = false;
cell = worksheet.Cells.Find("bc", null, options);
Console.WriteLine(cell == null ? "Not found" : $"Found at: {cell.Name}");
}
}
}
```
### See Also
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
