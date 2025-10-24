##FindOptions.SearchBackward
FindOptions property. Whether search backward for cells
## FindOptions.SearchBackward property
Whether search backward for cells.
```csharp
public bool SearchBackward { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsPropertySearchBackwardDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Setup sample data
worksheet.Cells["A1"].PutValue("abc");
worksheet.Cells["B2"].PutValue("abc");
worksheet.Cells["C3"].PutValue("abc");
FindOptions options = new FindOptions();
options.LookInType = LookInType.Values;
options.LookAtType = LookAtType.Contains;
// Search forward (default behavior)
options.SearchBackward = false;
Cell foundForward = worksheet.Cells.Find("abc", null, options);
Console.WriteLine($"Forward search found at: {foundForward.Name}");
// Search backward
options.SearchBackward = true;
Cell foundBackward = worksheet.Cells.Find("abc", null, options);
Console.WriteLine($"Backward search found at: {foundBackward.Name}");
}
}
}
```
### See Also
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
