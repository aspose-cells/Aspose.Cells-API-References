##Cells.Find
Cells method. Finds the cell containing with the input object
## Find(object, Cell) {#find}
Finds the cell containing with the input object.
```csharp
public Cell Find(object what, Cell previousCell)
```
| Parameter | Type | Description |
| --- | --- | --- |
| what | Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | Cell | Previous cell with the same object. This parameter can be set to null if searching from the start. |
### Return Value
Cell object.
### Remarks
Returns null (Nothing) if no cell is found.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodFindWithObjectCellDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some sample data
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(2.5);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(1.8);
worksheet.Cells["A4"].PutValue("Banana");
worksheet.Cells["B4"].PutValue(1.2);
// Find the cell containing "Orange"
Cell searchCell = null;
Cell foundCell = worksheet.Cells.Find("Orange", searchCell);
if (foundCell != null)
{
Console.WriteLine("Found 'Orange' at: " + foundCell.Name);
// Create and apply a style to the found cell
Style style = workbook.CreateStyle();
style.Font.Color = System.Drawing.Color.Red;
style.Font.IsBold = true;
foundCell.SetStyle(style);
}
// Save the workbook
workbook.Save("FindMethodDemo.xlsx");
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Find(object, Cell, FindOptions) {#find_1}
Finds the cell containing with the input object.
```csharp
public Cell Find(object what, Cell previousCell, FindOptions findOptions)
```
| Parameter | Type | Description |
| --- | --- | --- |
| what | Object | The object to search for. The type should be int,double,DateTime,string,bool. |
| previousCell | Cell | Previous cell with the same object. This parameter can be set to null if searching from the start. |
| findOptions | FindOptions | Find options |
### Return Value
Cell object.
### Remarks
Returns null (Nothing) if no cell is found.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodFindWithObjectCellFindOptionsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample data
worksheet.Cells["A1"].PutValue("abc");
worksheet.Cells["A2"].PutValue("def");
worksheet.Cells["A3"].PutValue("abc ");
// Create find options
FindOptions options = new FindOptions();
options.LookInType = LookInType.Values;
options.LookAtType = LookAtType.Contains;
// Find cell with value "abc "
Cell foundCell = worksheet.Cells.Find("abc ", null, options);
Console.WriteLine("Found cell: " + (foundCell != null ? foundCell.Name : "null"));
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [FindOptions](../../findoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
