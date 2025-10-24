##XlsbSaveOptions.XlsbSaveOptions
XlsbSaveOptions constructor. Creates xlsb file save options
## XlsbSaveOptions() {#constructor}
Creates xlsb file save options.
```csharp
public XlsbSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XlsbSaveOptionsMethodCtorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells["A1"].PutValue("Test Value");
XlsbSaveOptions saveOptions = new XlsbSaveOptions();
saveOptions.ExportAllColumnIndexes = true;
workbook.Save("output.xlsb", saveOptions);
}
}
}
```
### See Also
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## XlsbSaveOptions(SaveFormat) {#constructor_1}
Creates xlsb file save options.
```csharp
[Obsolete("Use XlsbSaveOptions() constructor instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public XlsbSaveOptions(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format . It must be xlsb. |
### Remarks
NOTE: This constructor is now obsolete. Instead, please use XlsbSaveOptions() constructor. This property will be removed 12 months later since January 2021. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* enum [SaveFormat](../../saveformat/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
