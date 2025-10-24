##XlsbSaveOptions.CompressionType
XlsbSaveOptions property. Gets and sets the compression type for ooxml file
## XlsbSaveOptions.CompressionType property
Gets and sets the compression type for ooxml file.
```csharp
public OoxmlCompressionType CompressionType { get; set; }
```
### Remarks
The default value is OoxmlCompressionType.Level6.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XlsbSaveOptionsPropertyCompressionTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Compression Test");
XlsbSaveOptions saveOptions = new XlsbSaveOptions
{
CompressionType = OoxmlCompressionType.Level6
};
workbook.Save("XlsbWithCompression.xlsb", saveOptions);
}
}
}
```
### See Also
* enum [OoxmlCompressionType](../../ooxmlcompressiontype/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
