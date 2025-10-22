##StyleFlag.FontName
StyleFlag property. Font name setting will be applied
## StyleFlag.FontName property
Font name setting will be applied.
```csharp
public bool FontName { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyFontNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create sample data
cells["A1"].PutValue("Product Name");
cells["B1"].PutValue("Price");
cells["A2"].PutValue("Laptop");
cells["B2"].PutValue(999.99);
cells["A3"].PutValue("Phone");
cells["B3"].PutValue(699.99);
// Create styles with different font names
Style headerStyle = workbook.CreateStyle();
headerStyle.Font.Name = "Arial";
headerStyle.Font.IsBold = true;
headerStyle.Font.Size = 14;
Style priceStyle = workbook.CreateStyle();
priceStyle.Font.Name = "Courier New";
priceStyle.Custom = "$#,##0.00";
// Apply header style with StyleFlag
Aspose.Cells.Range headerRange = cells.CreateRange(0, 0, 1, 2);
StyleFlag headerFlag = new StyleFlag();
headerFlag.FontName = true;
headerFlag.FontBold = true;
headerFlag.FontSize = true;
headerRange.ApplyStyle(headerStyle, headerFlag);
// Apply price style with StyleFlag focusing on FontName
Aspose.Cells.Range priceRange = cells.CreateRange(1, 1, 2, 1);
StyleFlag priceFlag = new StyleFlag();
priceFlag.FontName = true;
priceFlag.NumberFormat = true;
priceRange.ApplyStyle(priceStyle, priceFlag);
// Auto-fit columns for better visibility
worksheet.AutoFitColumns();
// Save the workbook
workbook.Save("FontNameDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
