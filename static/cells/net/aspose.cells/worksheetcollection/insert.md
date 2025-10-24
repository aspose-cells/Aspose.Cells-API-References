##WorksheetCollection.Insert
WorksheetCollection method. Insert a worksheet
## Insert(int, SheetType) {#insert}
Insert a worksheet.
```csharp
public Worksheet Insert(int index, SheetType sheetType)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The sheet index |
| sheetType | SheetType | The sheet type. |
### Return Value
Returns an inserted worksheet.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodInsertWithInt32SheetTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets.Insert(1, SheetType.Worksheet);
worksheet.Name = "InsertedSheet";
workbook.Worksheets[0].Cells["A1"].Value = "Referencing inserted sheet:";
workbook.Worksheets[0].Cells["A2"].Formula = "='InsertedSheet'!A1";
}
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Insert(int, SheetType, string) {#insert_1}
Insert a worksheet.
```csharp
public Worksheet Insert(int index, SheetType sheetType, string sheetName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | Int32 | The sheet index |
| sheetType | SheetType | The sheet type. |
| sheetName | String | The sheet name. |
### Return Value
Returns an inserted worksheet.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodInsertWithInt32SheetTypeStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Insert a new worksheet at index 0 with name "InsertedSheet"
workbook.Worksheets.Insert(0, SheetType.Worksheet, "InsertedSheet");
// Access the inserted worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Put some data in cell A1 of the inserted sheet
worksheet.Cells["A1"].PutValue("This sheet was inserted using Insert method");
// Save the workbook
workbook.Save("WorksheetInsertDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* enum [SheetType](../../sheettype/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
