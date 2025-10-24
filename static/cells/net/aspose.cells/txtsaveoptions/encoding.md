##TxtSaveOptions.Encoding
TxtSaveOptions property. Gets and sets the default encoding
## TxtSaveOptions.Encoding property
Gets and sets the default encoding.
```csharp
public Encoding Encoding { get; set; }
```
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class TxtSaveOptionsPropertyEncodingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["A2"].PutValue("World");
// Create TXT save options with ASCII encoding
TxtSaveOptions saveOptions = new TxtSaveOptions
{
Encoding = Encoding.ASCII,
Separator = '\t'
};
// Save the workbook with specified encoding
workbook.Save("output.txt", saveOptions);
Console.WriteLine("File saved with ASCII encoding");
}
}
}
```
### See Also
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
