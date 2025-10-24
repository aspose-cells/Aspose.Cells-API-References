##XpsSaveOptions.XpsSaveOptions
XpsSaveOptions constructor. Creates options for saving xps file
## XpsSaveOptions() {#constructor}
Creates options for saving xps file.
```csharp
public XpsSaveOptions()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XpsSaveOptionsMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("XPS Save Options Demo");
// Initialize XpsSaveOptions using constructor
XpsSaveOptions saveOptions = new XpsSaveOptions();
// Configure save options
saveOptions.OnePagePerSheet = true;
saveOptions.DefaultFont = "Arial";
saveOptions.PageIndex = 0;
saveOptions.PageCount = 1;
// Save workbook with options
workbook.Save("XpsSaveOptionsDemo.xps", saveOptions);
}
}
}
```
### See Also
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## XpsSaveOptions(SaveFormat) {#constructor_1}
Creates options for saving xps file.
```csharp
[Obsolete("Use XpsSaveOptions() constructor instead.")]
public XpsSaveOptions(SaveFormat saveFormat)
```
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | SaveFormat | The save format, it must be xps format. |
### Remarks
NOTE: This constructor is now obsolete. Instead, please use XpsSaveOptions() constructor. This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* enum [SaveFormat](../../saveformat/)
* class [XpsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
