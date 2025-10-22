##TxtSaveOptions.QuoteType
TxtSaveOptions property. Gets or sets how to quote values in the exported text file
## TxtSaveOptions.QuoteType property
Gets or sets how to quote values in the exported text file.
```csharp
public TxtValueQuoteType QuoteType { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsPropertyQuoteTypeDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Text");
worksheet.Cells["B1"].PutValue("123");
worksheet.Cells["A2"].PutValue("Another text");
worksheet.Cells["B2"].PutValue("=1+2");
// Save with QuoteType.Normal (default)
MemoryStream stream1 = new MemoryStream();
workbook.Save(stream1, new TxtSaveOptions()
{
Encoding = Encoding.ASCII
});
// Save with QuoteType.Always
MemoryStream stream2 = new MemoryStream();
workbook.Save(stream2, new TxtSaveOptions()
{
Encoding = Encoding.ASCII,
QuoteType = TxtValueQuoteType.Always
});
// Display sample output
Console.WriteLine("Normal QuoteType:");
Console.WriteLine(Encoding.ASCII.GetString(stream1.ToArray()));
Console.WriteLine("\nAlways QuoteType:");
Console.WriteLine(Encoding.ASCII.GetString(stream2.ToArray()));
}
}
}
```
### See Also
* enum [TxtValueQuoteType](../../txtvaluequotetype/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
