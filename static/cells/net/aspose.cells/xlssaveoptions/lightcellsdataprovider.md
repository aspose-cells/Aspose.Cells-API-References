##XlsSaveOptions.LightCellsDataProvider
XlsSaveOptions property. The data provider for saving workbook in light mode
## XlsSaveOptions.LightCellsDataProvider property
The data provider for saving workbook in light mode.
```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XlsSaveOptionsPropertyLightCellsDataProviderDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Create XLS save options
XlsSaveOptions saveOptions = new XlsSaveOptions();
// Set the LightCellsDataProvider
saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
// Save the workbook with LightCells mode
workbook.Save("output.xls", saveOptions);
}
}
public class CustomLightCellsDataProvider : LightCellsDataProvider
{
public bool IsGatherString()
{
return true;
}
public int NextCell()
{
return 0; // Only process first cell for demonstration
}
public int NextRow()
{
return 0; // Only process first row for demonstration
}
public void StartCell(Cell cell)
{
// Set a long string value to demonstrate LightCells handling
cell.PutValue(new string('X', 257));
}
public void StartRow(Row row)
{
// No special row handling needed for this demo
}
public bool StartSheet(int sheetIndex)
{
// No special sheet handling needed for this demo
return false;
}
}
}
```
### See Also
* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
