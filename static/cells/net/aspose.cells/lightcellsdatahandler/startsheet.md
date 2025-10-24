##LightCellsDataHandler.StartSheet
LightCellsDataHandler method. Starts to process a worksheet
## LightCellsDataHandler.StartSheet method
Starts to process a worksheet.
```csharp
public bool StartSheet(Worksheet sheet)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheet | Worksheet | the worksheet to read cells data. |
### Return Value
whether this sheet's cells data needs to be processed. false to ignore this sheet.
### Remarks
It will be called before reading cells data of a worksheet.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class LightCellsDataHandlerMethodStartSheetWithWorksheetDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
CustomLightCellsDataHandler handler = new CustomLightCellsDataHandler();
bool result = handler.StartSheet(worksheet);
Console.WriteLine($"StartSheet method returned: {result}");
Console.WriteLine($"Worksheet name after StartSheet: {worksheet.Name}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing StartSheet method: {ex.Message}");
}
workbook.Save("LightCellsDataHandlerStartSheetDemo.xlsx");
}
}
public class CustomLightCellsDataHandler : LightCellsDataHandler
{
public bool StartSheet(Worksheet sheet)
{
sheet.Name = "ModifiedByStartSheet";
return true;
}
public bool StartRow(int rowIndex) => true;
public bool ProcessRow(Row row) => true;
public bool StartCell(int columnIndex) => true;
public bool ProcessCell(Cell cell) => true;
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
