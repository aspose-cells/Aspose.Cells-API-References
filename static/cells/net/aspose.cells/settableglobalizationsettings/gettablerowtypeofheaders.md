##SettableGlobalizationSettings.GetTableRowTypeOfHeaders
SettableGlobalizationSettings method. Gets the type name of table rows that consists of the table header. Default is Headers so in formula Headers represents the table header
## SettableGlobalizationSettings.GetTableRowTypeOfHeaders method
Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header.
```csharp
public override string GetTableRowTypeOfHeaders()
```
### Return Value
the type name of table rows
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class SettableGlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom globalization settings
SettableGlobalizationSettings settings = new SettableGlobalizationSettings();
settings.SetTableRowTypeOfHeaders("CustomHeaders");
workbook.Settings.GlobalizationSettings = settings;
// Create sample table data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(15);
try
{
// Get the table row type for headers
string rowType = settings.GetTableRowTypeOfHeaders();
Console.WriteLine($"Table row type for headers: {rowType}");
// Create a ListObject (Table)
ListObject table = worksheet.ListObjects[worksheet.ListObjects.Add("A1", "B3", true)];
// Use the custom header reference in a formula
worksheet.Cells["C2"].Formula = "=COUNTA(Table1[#CustomHeaders])";
Console.WriteLine("Formula using custom headers reference: " + worksheet.Cells["C2"].Formula);
// Calculate the formula
workbook.CalculateFormula();
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTableRowTypeOfHeaders method: {ex.Message}");
}
workbook.Save("MethodGetTableRowTypeOfHeadersDemo.xlsx");
}
}
}
```
### See Also
* class [SettableGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
