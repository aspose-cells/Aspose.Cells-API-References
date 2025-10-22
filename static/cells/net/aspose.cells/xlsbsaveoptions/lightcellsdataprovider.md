##XlsbSaveOptions.LightCellsDataProvider
XlsbSaveOptions property. The data provider for saving workbook in light mode
## XlsbSaveOptions.LightCellsDataProvider property
The data provider for saving workbook in light mode.
```csharp
public LightCellsDataProvider LightCellsDataProvider { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class XlsbSaveOptionsPropertyLightCellsDataProviderDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
for (int i = 0; i < 10; i++)
{
worksheet.Cells[i, 0].PutValue($"Data {i}");
}
// Create XLSB save options
XlsbSaveOptions saveOptions = new XlsbSaveOptions();
saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();
// Save the workbook with LightCellsDataProvider
using (MemoryStream stream = new MemoryStream())
{
workbook.Save(stream, saveOptions);
// Verify the saved data
stream.Seek(0, SeekOrigin.Begin);
Workbook savedWorkbook = new Workbook(stream);
Console.WriteLine("Workbook saved successfully with LightCellsDataProvider");
}
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
// Implement cell iteration logic here
return -1; // Return -1 when no more cells
}
public int NextRow()
{
// Implement row iteration logic here
return -1; // Return -1 when no more rows
}
public void StartCell(Cell cell)
{
// Implement cell processing logic here
}
public void StartRow(Row row)
{
// Implement row processing logic here
}
public bool StartSheet(int sheetIndex)
{
// Implement sheet processing logic here
return true; // Return true to process the sheet
}
}
}
```
### See Also
* interface [LightCellsDataProvider](../../lightcellsdataprovider/)
* class [XlsbSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
