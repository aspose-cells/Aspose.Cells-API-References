##TableStyleCollection.DefaultTableStyleName
TableStyleCollection property. Gets and sets the default style name of the table
## TableStyleCollection.DefaultTableStyleName property
Gets and sets the default style name of the table.
```csharp
public string DefaultTableStyleName { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class TableStyleCollectionPropertyDefaultTableStyleNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the table styles collection
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
// Display the default table style name
Console.WriteLine("Default Table Style: " + tableStyles.DefaultTableStyleName);
// Change the default table style
tableStyles.DefaultTableStyleName = "TableStyleMedium9";
Console.WriteLine("New Default Table Style: " + tableStyles.DefaultTableStyleName);
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
