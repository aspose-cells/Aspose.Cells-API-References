##FindOptions.LookAtType
FindOptions property. Look at type
## FindOptions.LookAtType property
Look at type.
```csharp
public LookAtType LookAtType { get; set; }
```
### Remarks
When [`RegexKey`](../regexkey/) is true and user has specified the exact rule for the regex, for performance consideration this property should be set as EntireContent. Otherwise we will refactor the search key to ensure it can be matched according to the specific type. For example, when the type is Contains(this is the default value for this property), we will add wildcards at the beginning and end of the search key automatically. In this case, the regular expressions will become more complex and the performance will also decrease.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsPropertyLookAtTypeDemo
{
public static void Run()
{
// Create a workbook and add some data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Hello World");
worksheet.Cells["A2"].PutValue("=1+2"); // Formula
worksheet.Cells["A3"].PutValue("Partial match test");
worksheet.Cells["A4"].PutValue("=A1&A3"); // Formula concatenating cells
// Create find options with LookAtType.EntireContent
FindOptions options = new FindOptions
{
LookInType = LookInType.OnlyFormulas,
LookAtType = LookAtType.EntireContent
};
// Search for formula that exactly matches "=A1&A3"
Cell cell = worksheet.Cells.Find("=A1&A3", null, options);
Console.WriteLine("Found cell with exact formula match: " + (cell != null ? cell.Name : "null"));
// Change to partial matching
options.LookAtType = LookAtType.Contains;
cell = worksheet.Cells.Find("A3", null, options);
Console.WriteLine("Found cell containing 'A3' in formula: " + (cell != null ? cell.Name : "null"));
}
}
}
```
### See Also
* enum [LookAtType](../../lookattype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
