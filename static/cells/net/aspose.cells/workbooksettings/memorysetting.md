##WorkbookSettings.MemorySetting
WorkbookSettings property. Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets
## WorkbookSettings.MemorySetting property
Gets or sets the memory usage options. The new option will be taken as the default option for newly created worksheets but does not take effect for existing worksheets.
```csharp
public MemorySetting MemorySetting { get; set; }
```
### Remarks
For more details about memory mode, please see [`MemorySetting`](../../cells/memorysetting/).
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyMemorySettingDemo
{
public static void Run()
{
// Create a new workbook with memory preference setting
Workbook wb = new Workbook();
wb.Settings.MemorySetting = MemorySetting.MemoryPreference;
// Access the first worksheet and add some data
Worksheet sheet = wb.Worksheets[0];
sheet.Cells["A1"].PutValue("Memory Setting Demo");
sheet.Cells["A2"].PutValue(DateTime.Now.ToString());
// Save to memory stream with PDF format
using (MemoryStream ms = new MemoryStream())
{
wb.Save(ms, SaveFormat.Pdf);
Console.WriteLine("Workbook saved to PDF with MemoryPreference setting");
}
}
}
}
```
### See Also
* enum [MemorySetting](../../memorysetting/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
