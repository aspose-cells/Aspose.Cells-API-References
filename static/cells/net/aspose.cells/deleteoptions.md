##Class DeleteOptions
Aspose.Cells.DeleteOptions class. Represents the setting of deleting rows/columns
## DeleteOptions class
Represents the setting of deleting rows/columns.
```csharp
public class DeleteOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [DeleteOptions](deleteoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [FormulaChangeMonitor](../../aspose.cells/deleteoptions/formulachangemonitor/) { get; set; } | Gets/sets the monitor for tracking changes caused by the deletion. |
| [UpdateReference](../../aspose.cells/deleteoptions/updatereference/) { get; set; } | Indicates if update references in other worksheets. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DeleteOptionsDemo
{
public static void DeleteOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add some data to the worksheet
sheet.Cells["A1"].PutValue("Item");
sheet.Cells["A2"].PutValue("Apple");
sheet.Cells["A3"].PutValue("Banana");
sheet.Cells["A4"].PutValue("Cherry");
// Display the original data
Console.WriteLine("Original Data:");
for (int i = 1; i <= 4; i++)
{
Console.WriteLine(sheet.Cells[$"A{i}"].Value);
}
// Create DeleteOptions
DeleteOptions options = new DeleteOptions
{
UpdateReference = true // Set to true to update references in other worksheets
};
// Delete the second row (Banana)
sheet.Cells.DeleteRow(2, options.UpdateReference);
// Display the data after deletion
Console.WriteLine("\nData After Deletion:");
for (int i = 1; i <= 3; i++)
{
Console.WriteLine(sheet.Cells[$"A{i}"].Value);
}
// Save the workbook
workbook.Save("DeleteOptionsExample.xlsx");
workbook.Save("DeleteOptionsExample.pdf");
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
