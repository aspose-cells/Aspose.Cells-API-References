##ReferredArea.GetValue
ReferredArea method. Gets cell value with given offset from the topleft of this area
## GetValue(int, int) {#getvalue}
Gets cell value with given offset from the top-left of this area.
```csharp
public object GetValue(int rowOffset, int colOffset)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | row offset from the start row of this area |
| colOffset | Int32 | column offset from the start row of this area |
### Return Value
"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaMethodGetValueWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue(5);
Cell cell = worksheet.Cells["C1"];
cell.Formula = "=A1";
workbook.CalculateFormula();
ReferredAreaCollection referredAreas = cell.GetPrecedents();
if (referredAreas.Count > 0)
{
object value = referredAreas[0].GetValue(0, 0);
Console.WriteLine("Value at (0,0): " + value);
}
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetValue(int, int, bool) {#getvalue_1}
Gets cell value with given offset from the top-left of this area.
```csharp
public object GetValue(int rowOffset, int colOffset, bool calculateFormulas)
```
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | row offset from the start row of this area |
| colOffset | Int32 | column offset from the start row of this area |
| calculateFormulas | Boolean | Whether calculate it recursively if the specified reference is formula |
### Return Value
"#REF!" if this area is invalid; "#N/A" if given offset out of this area; Otherwise return the cell value at given position.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ReferredAreaMethodGetValueWithInt32Int32BooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
sheet.Cells["A1"].PutValue(100);
sheet.Cells["B1"].PutValue(200);
workbook.Worksheets.Names.Add("TestRange");
Name name = workbook.Worksheets.Names["TestRange"];
name.RefersTo = "=Sheet1!$A$1:$B$1";
ReferredArea ra = name.GetReferredAreas(true)[0];
object result = ra.GetValue(0, 0, true);
Console.WriteLine("Obtained value: " + result);
}
}
}
```
### See Also
* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
