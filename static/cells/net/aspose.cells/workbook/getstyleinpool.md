##Workbook.GetStyleInPool
Workbook method. Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells
## Workbook.GetStyleInPool method
Gets the style in the style pool. All styles in the workbook will be gathered into a pool. There is only a simple reference index in the cells.
```csharp
public Style GetStyleInPool(int index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The index. |
### Return Value
The style in the pool corresponds to given index, may be null.
### Remarks
If the returned style is changed, the style of all cells(which refers to this style) will be changed.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodGetStyleInPoolWithInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Access first worksheet and add some sample data
Worksheet ws = wb.Worksheets[0];
ws.Cells["A1"].PutValue("Sample Data");
ws.Cells["A2"].PutValue(123.45);
ws.Cells["A3"].PutValue(DateTime.Now);
// Apply some styles
Style style1 = wb.CreateStyle();
style1.Custom = "$#,##0.00";
ws.Cells["A2"].SetStyle(style1);
Style style2 = wb.CreateStyle();
style2.Custom = "yyyy-mm-dd";
ws.Cells["A3"].SetStyle(style2);
// Save to memory stream
using (MemoryStream ms = new MemoryStream())
{
wb.Save(ms, SaveFormat.Xlsx);
// Reload workbook from stream
ms.Position = 0;
Workbook reloadWb = new Workbook(ms);
// Get and display styles from style pool
int count = reloadWb.CountOfStylesInPool;
Console.WriteLine($"Styles in pool: {count}");
for (int i = 0; i < count; i++)
{
Style style = reloadWb.GetStyleInPool(i);
Console.WriteLine($"Style {i}: CustomFormat={style.Custom}");
}
}
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
