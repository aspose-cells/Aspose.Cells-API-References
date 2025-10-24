##HtmlSaveOptions.Encoding
HtmlSaveOptions property. If not setuse Encoding.UTF8 as default enconding type
## HtmlSaveOptions.Encoding property
If not set,use Encoding.UTF8 as default enconding type.
```csharp
public Encoding Encoding { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyEncodingDemo
{
private class SheetStreamProvider : IStreamProvider
{
private readonly MemoryStream _sheet1Stream;
private readonly MemoryStream _sheet2Stream;
private int _currentIndex = 0;
public SheetStreamProvider(MemoryStream sheet1Stream, MemoryStream sheet2Stream)
{
_sheet1Stream = sheet1Stream;
_sheet2Stream = sheet2Stream;
}
public void InitStream(StreamProviderOptions options)
{
// Initialization if needed
}
public Stream GetStream(string sheetName)
{
return _currentIndex++ == 0 ? _sheet1Stream : _sheet2Stream;
}
public void CloseStream(StreamProviderOptions options)
{
options.Stream?.Flush();
}
}
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add sample data to worksheets
workbook.Worksheets[0].Cells[0, 0].PutValue("Sample content in Sheet1");
workbook.Worksheets.Add("Sheet2").Cells[0, 0].PutValue("Sample content in Sheet2");
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set the encoding to UTF8
saveOptions.Encoding = Encoding.UTF8;
// Create memory streams for output
using (MemoryStream sheet1Stream = new MemoryStream())
using (MemoryStream sheet2Stream = new MemoryStream())
{
// Create a stream provider to handle multiple sheets
SheetStreamProvider streamProvider = new SheetStreamProvider(sheet1Stream, sheet2Stream);
saveOptions.StreamProvider = streamProvider;
// Save the workbook with HTML options
workbook.Save(new MemoryStream(), saveOptions);
// Verify the content was saved with UTF8 encoding
string sheet1Content = Encoding.UTF8.GetString(sheet1Stream.ToArray());
string sheet2Content = Encoding.UTF8.GetString(sheet2Stream.ToArray());
Console.WriteLine("Sheet1 content contains text: " +
sheet1Content.Contains("Sample content in Sheet1"));
Console.WriteLine("Sheet2 content contains text: " +
sheet2Content.Contains("Sample content in Sheet2"));
}
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
