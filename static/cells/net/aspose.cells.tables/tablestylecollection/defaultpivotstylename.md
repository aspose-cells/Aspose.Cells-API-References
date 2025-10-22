##TableStyleCollection.DefaultPivotStyleName
TableStyleCollection property. Gets and sets the default style name of pivot table
## TableStyleCollection.DefaultPivotStyleName property
Gets and sets the default style name of pivot table .
```csharp
public string DefaultPivotStyleName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TableStyleCollectionPropertyDefaultPivotStyleNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the table styles collection
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
// Display default pivot style name
Console.WriteLine("Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
// Change the default pivot style
tableStyles.DefaultPivotStyleName = "PivotStyleDark2";
// Verify the change
Console.WriteLine("Updated Default Pivot Style: " + tableStyles.DefaultPivotStyleName);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
