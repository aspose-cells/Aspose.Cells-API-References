##NameCollection.Filter
NameCollection method. Gets all defined name by scope
## NameCollection.Filter method
Gets all defined name by scope.
```csharp
public Name[] Filter(NameScopeType type, int sheetIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | NameScopeType | The scope type. |
| sheetIndex | Int32 | The sheet index. Only effects when scope type is Worksheet |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class NameCollectionMethodFilterWithNameScopeTypeInt32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some names to the workbook and worksheets
workbook.Worksheets.Names.Add("GlobalName");
Worksheet worksheet1 = workbook.Worksheets[0];
workbook.Worksheets.Names.Add("Sheet1Name");
Worksheet worksheet2 = workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Names.Add("Sheet2Name");
// Filter names by scope type and sheet index
Name[] workbookScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Workbook, -1);
Name[] worksheetScopeNames = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, -1);
Name[] sheet1Names = workbook.Worksheets.Names.Filter(NameScopeType.Worksheet, 0);
// Output results
Console.WriteLine($"Workbook-scoped names count: {workbookScopeNames.Length}");
Console.WriteLine($"Worksheet-scoped names count: {worksheetScopeNames.Length}");
Console.WriteLine($"Sheet1 names count: {sheet1Names.Length}");
}
}
}
```
### See Also
* class [Name](../../name/)
* enum [NameScopeType](../../namescopetype/)
* class [NameCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
