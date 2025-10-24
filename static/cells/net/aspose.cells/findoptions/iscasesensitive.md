##FindOptions.IsCaseSensitive
FindOptions property. Indicates if the searched string is case sensitive
## FindOptions.IsCaseSensitive property
Indicates if the searched string is case sensitive.
```csharp
[Obsolete("Use FindOptions.CaseSensitive property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCaseSensitive { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use FindOptions.CaseSensitive property. This property will be removed 12 months later since June 2010. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FindOptionsPropertyIsCaseSensitiveDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data
worksheet.Cells["A1"].PutValue("ABC");
worksheet.Cells["A2"].PutValue("abc");
worksheet.Cells["A3"].PutValue("AbC");
FindOptions options = new FindOptions();
options.IsCaseSensitive = true;
// Find case-sensitive match
Cell cell = worksheet.Cells.Find("abc", null, options);
Console.WriteLine("Case-sensitive search for 'abc' found at: " +
(cell != null ? cell.Name : "No match"));
}
}
}
```
### See Also
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
