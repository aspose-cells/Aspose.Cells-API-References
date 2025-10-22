##Protection.AllowUsingPivotTable
Protection property. Represents if the user is allowed to manipulate pivot tables on a protected worksheet
## Protection.AllowUsingPivotTable property
Represents if the user is allowed to manipulate pivot tables on a protected worksheet.
```csharp
public bool AllowUsingPivotTable { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class ProtectionPropertyAllowUsingPivotTableDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Enable worksheet protection
Protection protection = worksheet.Protection;
protection.AllowUsingPivotTable = true;
worksheet.Protect(ProtectionType.All);
// Verify the setting
Console.WriteLine("AllowUsingPivotTable is set to: " + protection.AllowUsingPivotTable);
// Create a pivot table to demonstrate the functionality
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(150);
// Create pivot table with correct parameters
int pivotIndex = worksheet.PivotTables.Add("A1:B3", "C1", "PivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Save the workbook
workbook.Save("ProtectionPropertyAllowUsingPivotTableDemo.xlsx");
}
}
}
```
### See Also
* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
