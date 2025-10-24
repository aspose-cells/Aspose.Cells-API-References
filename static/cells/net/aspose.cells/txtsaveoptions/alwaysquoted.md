##TxtSaveOptions.AlwaysQuoted
TxtSaveOptions property. Indicates whether always adding  for each field. If true then all values will be quoted If false then values will only be quoted when neededfor example when values contain special characters such as   n or separator character. Default is false
## TxtSaveOptions.AlwaysQuoted property
Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will only be quoted when needed(for example, when values contain special characters such as '"' , '\n' or separator character). Default is false.
```csharp
[Obsolete("Use QuoteType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool AlwaysQuoted { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use QuoteType property instead. This property will be removed 12 months later since August 2012. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsPropertyAlwaysQuotedDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Laptop");
worksheet.Cells["B2"].PutValue(1200.50);
worksheet.Cells["A3"].PutValue("Phone");
worksheet.Cells["B3"].PutValue(899.99);
// Create TxtSaveOptions with AlwaysQuoted set to true
TxtSaveOptions saveOptions = new TxtSaveOptions
{
Separator = ',',
AlwaysQuoted = true,
QuoteType = TxtValueQuoteType.Always
};
// Save with quotes around all values
workbook.Save("AlwaysQuoted_True.txt", saveOptions);
// Change to false and save again
saveOptions.AlwaysQuoted = false;
workbook.Save("AlwaysQuoted_False.txt", saveOptions);
Console.WriteLine("Files saved with different AlwaysQuoted settings.");
}
}
}
```
### See Also
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
