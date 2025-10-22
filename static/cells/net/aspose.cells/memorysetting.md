##Enum MemorySetting
Aspose.Cells.MemorySetting enum. Memory usage modes for cells data model
## MemorySetting enumeration
Memory usage modes for cells data model.
```csharp
public enum MemorySetting
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Normal | `0` | Default mode for cells model. |
| MemoryPreference | `1` | Memory performance preferable. |
| FileCache | `2` | Memory performance preferable and using file instead of memory to maintain the cells data. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class MemorySettingDemo
{
public static void MemorySettingExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the workbook settings
WorkbookSettings settings = workbook.Settings;
// Set the memory usage option to MemoryPreference
settings.MemorySetting = MemorySetting.MemoryPreference;
// Create a worksheet and add some data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Data");
worksheet.Cells["A2"].PutValue(123);
// Save the workbook
workbook.Save("MemorySettingExample.xlsx");
Console.WriteLine("Workbook saved with MemorySetting.MemoryPreference.");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
