##PivotTable.AltTextDescription
PivotTable property. Gets the description of the alt text
## PivotTable.AltTextDescription property
Gets the description of the alt text.
```csharp
public string AltTextDescription { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyAltTextDescriptionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(3000);
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display the current alt text description
Console.WriteLine("Current AltTextDescription: " + pivotTable.AltTextDescription);
// Set a new alt text description
pivotTable.AltTextDescription = "Sales data by product category";
// Save the workbook
workbook.Save("PivotTableAltTextDescriptionDemo.xlsx");
// Display the new alt text description
Console.WriteLine("New AltTextDescription: " + pivotTable.AltTextDescription);
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
