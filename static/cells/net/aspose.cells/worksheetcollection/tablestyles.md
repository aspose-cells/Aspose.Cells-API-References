##WorksheetCollection.TableStyles
WorksheetCollection property. Gets TableStyles object
## WorksheetCollection.TableStyles property
Gets `TableStyles` object.
```csharp
public TableStyleCollection TableStyles { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;
namespace AsposeCellsExamples
{
public class WorksheetCollectionPropertyTableStylesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some worksheets
workbook.Worksheets.Add("Sheet1");
workbook.Worksheets.Add("Sheet2");
// Create and add table styles
int styleIndex1 = workbook.Worksheets.TableStyles.AddTableStyle("Style1");
TableStyle style1 = workbook.Worksheets.TableStyles[styleIndex1];
int styleIndex2 = workbook.Worksheets.TableStyles.AddTableStyle("Style2");
TableStyle style2 = workbook.Worksheets.TableStyles[styleIndex2];
// Display the count of table styles
Console.WriteLine("Table styles count: " + workbook.Worksheets.TableStyles.Count);
// Remove one style
workbook.Worksheets.TableStyles.RemoveAt(0);
// Display updated count
Console.WriteLine("Table styles count after removal: " + workbook.Worksheets.TableStyles.Count);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [TableStyleCollection](../../../aspose.cells.tables/tablestylecollection/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
