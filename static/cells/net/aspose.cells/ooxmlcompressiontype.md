##Enum OoxmlCompressionType
Aspose.Cells.OoxmlCompressionType enum. The Ooxml compression type
## OoxmlCompressionType enumeration
The Ooxml compression type
```csharp
public enum OoxmlCompressionType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Level1 | `1` | The fastest but least effective compression. |
| Level2 | `2` | A little slower, but better, than level 1. |
| Level3 | `3` | A little slower, but better, than level 2. |
| Level4 | `4` | A little slower, but better, than level 3. |
| Level5 | `5` | A little slower than level 4, but with better compression. |
| Level6 | `6` | A good balance of speed and compression efficiency. |
| Level7 | `7` | Pretty good compression! |
| Level8 | `8` | Better compression than Level7! |
| Level9 | `9` | The "best" compression, where best means greatest reduction in size of the input data stream. This is also the slowest compression. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class OoxmlCompressionTypeDemo
{
public static void OoxmlCompressionTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A2"].PutValue(123);
worksheet.Cells["A3"].PutValue(456);
// Create OoxmlSaveOptions and set the compression type
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.CompressionType = OoxmlCompressionType.Level6; // A good balance of speed and compression efficiency
// Save the workbook with the specified compression type
workbook.Save("OoxmlCompressionTypeExample.xlsx", saveOptions);
Console.WriteLine("Workbook saved with OoxmlCompressionType.Level6 compression.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
