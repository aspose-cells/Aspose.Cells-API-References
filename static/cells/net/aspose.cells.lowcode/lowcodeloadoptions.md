##Class LowCodeLoadOptions
Aspose.Cells.LowCode.LowCodeLoadOptions class. Options for loading template file
## LowCodeLoadOptions class
Options for loading template file.
```csharp
public class LowCodeLoadOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [LowCodeLoadOptions](lowcodeloadoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [InputFile](../../aspose.cells.lowcode/lowcodeloadoptions/inputfile/) { get; set; } | Gets and sets the file(with path if needed) of the template. |
| [InputStream](../../aspose.cells.lowcode/lowcodeloadoptions/inputstream/) { get; set; } | Gets and sets the Stream of the template. |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class LowCodeClassLowCodeLoadOptionsDemo
{
public static void Run()
{
// Create a sample stream (in-memory for demo purposes)
using (MemoryStream stream = new MemoryStream())
{
// Create a new workbook and save to stream for demo
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet1");
workbook.Save(stream, SaveFormat.Xlsx);
// Reset stream position
stream.Position = 0;
// Create and use LowCodeLoadOptions
var loadOptions = new LowCodeLoadOptions()
{
InputStream = stream
};
// Example usage - would typically be passed to a processing method
Console.WriteLine($"Loading with LowCode options from stream of length: {loadOptions.InputStream.Length}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
