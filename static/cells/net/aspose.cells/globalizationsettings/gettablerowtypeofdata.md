##GlobalizationSettings.GetTableRowTypeOfData
GlobalizationSettings method. Gets the type name of table rows that consists of data region of referenced table. Default is Data so in formula Data represents the data region of the table
## GlobalizationSettings.GetTableRowTypeOfData method
Gets the type name of table rows that consists of data region of referenced table. Default is "Data", so in formula "#Data" represents the data region of the table.
```csharp
public virtual string GetTableRowTypeOfData()
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
public class CustomGlobalizationSettings1 : GlobalizationSettings
{
public override string GetTableRowTypeOfData()
{
return "MyData";
}
}
public class GlobalizationSettingsMethodGetTableRowTypeOfDataDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
workbook.Settings.GlobalizationSettings = new CustomGlobalizationSettings();
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(2.5);
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["B3"].PutValue(1.8);
// Fixed ListObjects.Add parameters to use correct overload
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.ShowHeaderRow = true;
table.DisplayName = "ProductTable";
table.ShowTotals = true;
table.ListColumns[1].TotalsCalculation = TotalsCalculation.Sum;
Cell formulaCell = worksheet.Cells["B5"];
formulaCell.Formula = "=SUM(ProductTable[#MyData])";
workbook.CalculateFormula();
Console.WriteLine($"Total price calculated: {formulaCell.Value}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetTableRowTypeOfData method: {ex.Message}");
}
workbook.Save("MethodGetTableRowTypeOfDataDemo.xlsx");
}
}
}
```
### See Also
* class [GlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
