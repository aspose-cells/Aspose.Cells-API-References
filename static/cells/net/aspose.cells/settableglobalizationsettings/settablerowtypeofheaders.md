##SettableGlobalizationSettings.SetTableRowTypeOfHeaders
SettableGlobalizationSettings method. Sets the type name of table rows that consists of the table header
## SettableGlobalizationSettings.SetTableRowTypeOfHeaders method
Sets the type name of table rows that consists of the table header.
```csharp
public void SetTableRowTypeOfHeaders(string name)
```
| Parameter | Type | Description |
| --- | --- | --- |
| name | String | the type name of table rows |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class SettableGlobalizationSettingsMethodSetTableRowTypeOfHeadersWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a table and add some data
Cells cells = worksheet.Cells;
cells["A1"].PutValue("Header1");
cells["B1"].PutValue("Header2");
cells["A2"].PutValue("Value1");
cells["B2"].PutValue("Value2");
// Create a ListObject (Table)
int index = worksheet.ListObjects.Add(0, 0, 1, 1, true);
ListObject table = worksheet.ListObjects[index];
table.ShowTotals = true;
// Create SettableGlobalizationSettings instance
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
try
{
// Call SetTableRowTypeOfHeaders with custom header type name
settings.SetTableRowTypeOfHeaders("CustomHeaders");
// Apply the settings to the workbook
workbook.Settings.GlobalizationSettings = settings;
Console.WriteLine("Table header type name set to: CustomHeaders");
Console.WriteLine("In formulas, '#CustomHeaders' will now represent the table header");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetTableRowTypeOfHeaders method: {ex.Message}");
}
// Save the workbook
workbook.Save("SetTableRowTypeOfHeadersDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
