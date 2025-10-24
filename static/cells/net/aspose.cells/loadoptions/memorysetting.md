##LoadOptions.MemorySetting
LoadOptions property. Gets or sets the memory mode for loaded workbook
## LoadOptions.MemorySetting property
Gets or sets the memory mode for loaded workbook.
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
public class LoadOptionsPropertyMemorySettingDemo
{
public static void Run()
{
// Create load options with memory preference setting
LoadOptions loadOptions = new LoadOptions(LoadFormat.Auto);
loadOptions.MemorySetting = MemorySetting.MemoryPreference;
// Load workbook with memory optimized settings
Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
// Access worksheet and add some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Memory Setting Demo");
worksheet.Cells["A2"].PutValue(DateTime.Now.ToString());
// Save the workbook
workbook.Save("MemorySettingDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Workbook saved with MemoryPreference setting.");
}
}
}
```
### See Also
* enum [MemorySetting](../../memorysetting/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
