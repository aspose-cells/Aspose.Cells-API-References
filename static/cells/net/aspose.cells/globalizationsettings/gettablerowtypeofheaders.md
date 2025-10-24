##GlobalizationSettings.GetTableRowTypeOfHeaders
GlobalizationSettings method. Gets the type name of table rows that consists of the table header. Default is Headers so in formula Headers represents the table header
## GlobalizationSettings.GetTableRowTypeOfHeaders method
Gets the type name of table rows that consists of the table header. Default is "Headers", so in formula "#Headers" represents the table header.
```csharp
public virtual string GetTableRowTypeOfHeaders()
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
public class GlobalizationSettingsMethodGetTableRowTypeOfHeadersDemo
{
public class CustomGlobalizationSettings : GlobalizationSettings
{
public override string GetTableRowTypeOfHeaders()
{
return "MyHeaders";
}
}
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Price";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["B2"].Value = 2.5;
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["B3"].Value = 1.8;
// Fixed ListObject creation by handling return value from Add()
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
// Use DisplayName property instead of Name
table.DisplayName = "FruitTable";
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
try
{
worksheet.Cells["A5"].Formula = "=COUNTA(FruitTable[#MyHeaders])";
workbook.CalculateFormula();
Console.WriteLine("Method executed successfully. Header count: " + worksheet.Cells["A5"].Value);
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
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
