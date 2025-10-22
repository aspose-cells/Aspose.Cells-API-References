##TableStyleElement.Size
TableStyleElement property. Number of rows or columns in a single band of striping. Applies only when type is firstRowStripe secondRowStripe firstColumnStripe or secondColumnStripe
## TableStyleElement.Size property
Number of rows or columns in a single band of striping. Applies only when type is firstRowStripe, secondRowStripe, firstColumnStripe, or secondColumnStripe.
```csharp
public int Size { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class TableStyleElementPropertySizeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a table
for (int i = 0; i < 10; i++)
{
for (int j = 0; j < 5; j++)
{
worksheet.Cells[i, j].PutValue($"Data {i},{j}");
}
}
// Create a table
int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
ListObject table = worksheet.ListObjects[tableIndex];
table.TableStyleType = TableStyleType.TableStyleMedium9;
// Create a table style using the workbook's style collection
TableStyleCollection styleCollection = workbook.Worksheets.TableStyles;
int styleIndex = styleCollection.AddTableStyle("CustomStyle");
TableStyle style = styleCollection[styleIndex];
table.TableStyleName = style.Name;
// Add stripe elements to demonstrate Size property
style.TableStyleElements.Add(TableStyleElementType.FirstRowStripe);
style.TableStyleElements.Add(TableStyleElementType.SecondRowStripe);
// Access the stripe elements
TableStyleElement firstStripe = style.TableStyleElements[TableStyleElementType.FirstRowStripe];
TableStyleElement secondStripe = style.TableStyleElements[TableStyleElementType.SecondRowStripe];
// Display current Size values
Console.WriteLine("Initial First Stripe Size: " + firstStripe.Size);
Console.WriteLine("Initial Second Stripe Size: " + secondStripe.Size);
// Modify the stripe sizes
firstStripe.Size = 2;
secondStripe.Size = 3;
// Display modified values
Console.WriteLine("Modified First Stripe Size: " + firstStripe.Size);
Console.WriteLine("Modified Second Stripe Size: " + secondStripe.Size);
// Save the workbook to see the effects
workbook.Save("TableStyleElementSizeDemo.xlsx");
}
}
}
```
### See Also
* class [TableStyleElement](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
