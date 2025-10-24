##LoadOptions.StandardFont
LoadOptions property. Sets the default standard font name
## LoadOptions.StandardFont property
Sets the default standard font name
```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use DefaultStyleSettings. This property will be removed 12 months later since March 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyStandardFontDemo
{
public static void Run()
{
// Create a sample Excel file in memory
MemoryStream ms = new MemoryStream();
using (Workbook workbook = new Workbook())
{
workbook.Worksheets[0].Cells["A1"].PutValue("Standard Font Test");
workbook.Save(ms, SaveFormat.Xlsx);
}
ms.Position = 0;
// Set load options with StandardFont
LoadOptions loadOptions = new LoadOptions();
loadOptions.StandardFont = "SimSun";
// Load workbook with the specified font
Workbook workbookWithFont = new Workbook(ms, loadOptions);
// Demonstrate the font is set by checking the default style
Console.WriteLine("Default font after loading: " +
workbookWithFont.DefaultStyle.Font.Name);
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
