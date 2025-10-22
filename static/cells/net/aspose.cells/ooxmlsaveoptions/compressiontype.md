##OoxmlSaveOptions.CompressionType
OoxmlSaveOptions property. Gets and sets the compression type for ooxml file
## OoxmlSaveOptions.CompressionType property
Gets and sets the compression type for ooxml file.
```csharp
public OoxmlCompressionType CompressionType { get; set; }
```
### Remarks
The default value is OoxmlCompressionType.Level2.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OoxmlSaveOptionsPropertyCompressionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Compression Test");
worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.CompressionType = OoxmlCompressionType.Level6;
workbook.Save("CompressionDemo.xlsx", saveOptions);
Console.WriteLine("Workbook saved with Level6 compression.");
}
}
}
```
### See Also
* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
