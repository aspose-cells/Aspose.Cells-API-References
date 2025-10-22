##OoxmlSaveOptions.EnableZip64
OoxmlSaveOptions property. Always use ZIP64 extensions when writing zip archives even when unnecessary
## OoxmlSaveOptions.EnableZip64 property
Always use ZIP64 extensions when writing zip archives, even when unnecessary.
```csharp
public bool EnableZip64 { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class OoxmlSaveOptionsPropertyEnableZip64Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].PutValue("Sample data for Zip64 demonstration");
OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
saveOptions.EnableZip64 = true;
workbook.Save("output_with_zip64.xlsx", saveOptions);
}
}
}
```
### See Also
* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
