##TableStyleCollection.GetBuiltinTableStyle
TableStyleCollection method. Gets the builtin table style
## TableStyleCollection.GetBuiltinTableStyle method
Gets the builtin table style
```csharp
public TableStyle GetBuiltinTableStyle(TableStyleType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | TableStyleType | The builtin table style type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Tables;
using System;
public class TableStyleCollectionMethodGetBuiltinTableStyleWithTableStyleTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to create a table
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create a table
int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
Aspose.Cells.Tables.ListObject table = worksheet.ListObjects[tableIndex];
try
{
// Get the table style collection
TableStyleCollection tableStyles = workbook.Worksheets.TableStyles;
// Call GetBuiltinTableStyle with TableStyleType parameter
TableStyle builtinStyle = tableStyles.GetBuiltinTableStyle(TableStyleType.TableStyleMedium2);
// Apply the built-in style to our table
table.TableStyleName = builtinStyle.Name;
Console.WriteLine($"Applied built-in table style: {builtinStyle.Name}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetBuiltinTableStyle method: {ex.Message}");
}
// Save the workbook
workbook.Save("TableStyleCollectionMethodGetBuiltinTableStyleDemo.xlsx");
}
}
}
```
### See Also
* class [TableStyle](../../tablestyle/)
* enum [TableStyleType](../../tablestyletype/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)
