##WorksheetCollection.Add
WorksheetCollection method. Adds a worksheet to the collection
## Add(SheetType) {#add_2}
Adds a worksheet to the collection.
```csharp
public int Add(SheetType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | SheetType | Worksheet type. |
### Return Value
[`Worksheet`](../../worksheet/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodAddWithSheetTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Add a new chart sheet using SheetType parameter
workbook.Worksheets.Add(SheetType.Chart);
// Add data to the first worksheet
Cells cells = workbook.Worksheets[0].Cells;
cells["C2"].PutValue(5000);
cells["C3"].PutValue(3000);
cells["C4"].PutValue(4000);
cells["C5"].PutValue(5000);
cells["C6"].PutValue(6000);
// Create chart in the chart sheet
Aspose.Cells.Charts.ChartCollection charts = workbook.Worksheets[1].Charts;
int chartIndex = charts.Add(Aspose.Cells.Charts.ChartType.Column, 10, 10, 20, 20);
Aspose.Cells.Charts.Chart chart = charts[chartIndex];
chart.NSeries.Add("Sheet1!C2:C6", true);
// Save the workbook (optional)
// workbook.Save("output.xlsx");
}
}
}
```
### See Also
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add() {#add_1}
Adds a worksheet to the collection.
```csharp
public int Add()
```
### Return Value
[`Worksheet`](../../worksheet/) object index.
### See Also
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(string) {#add}
Adds a worksheet to the collection.
```csharp
public Worksheet Add(string sheetName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sheetName | String | Worksheet name |
### Return Value
[`Worksheet`](../../worksheet/) object.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodAddWithStringDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet worksheet = wb.Worksheets.Add("NewSheet");
// Add data to the new worksheet
worksheet.Cells["A1"].PutValue("Worksheet added successfully!");
// Save the workbook
wb.Save("WorksheetCollectionMethodAddWithStringDemo_output.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
