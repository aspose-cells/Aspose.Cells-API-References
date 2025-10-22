##WorksheetCollection.GetSheetByCodeName
WorksheetCollection method. Gets the worksheet by the code name
## WorksheetCollection.GetSheetByCodeName method
Gets the worksheet by the code name.
```csharp
public Worksheet GetSheetByCodeName(string codeName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| codeName | String | Worksheet code name. |
### Return Value
The element with the specified code name.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetCollectionMethodGetSheetByCodeNameWithStringDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add worksheets and set their code names
Worksheet sheet1 = workbook.Worksheets.Add("Sheet1");
sheet1.CodeName = "MainSheet";
Worksheet sheet2 = workbook.Worksheets.Add("Sheet2");
sheet2.CodeName = "DataSheet";
// Get worksheet by code name
Worksheet mainSheet = workbook.Worksheets.GetSheetByCodeName("MainSheet");
Worksheet dataSheet = workbook.Worksheets.GetSheetByCodeName("DataSheet");
// Demonstrate usage by writing to cells
mainSheet.Cells["A1"].PutValue("This is Main Sheet");
dataSheet.Cells["A1"].PutValue("This is Data Sheet");
// Save the workbook
workbook.Save("GetSheetByCodeNameDemo.xlsx");
}
}
}
```
### See Also
* class [Worksheet](../../worksheet/)
* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
