##Workbook.CreateBuiltinStyle
Workbook method. Creates builtin style by given type
## Workbook.CreateBuiltinStyle method
Creates built-in style by given type.
```csharp
public Style CreateBuiltinStyle(BuiltinStyleType type)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | BuiltinStyleType | The builtin style stype. |
### Return Value
[`Style`](../../style/) object
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookMethodCreateBuiltinStyleWithBuiltinStyleTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Apply Good built-in style
workbook.Worksheets[0].Cells["A1"].PutValue("Good");
Style goodStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Good);
workbook.Worksheets[0].Cells["A1"].SetStyle(goodStyle);
// Apply Neutral built-in style
workbook.Worksheets[0].Cells["B2"].PutValue("Neutral");
Style neutralStyle = workbook.CreateBuiltinStyle(BuiltinStyleType.Neutral);
workbook.Worksheets[0].Cells["B2"].SetStyle(neutralStyle);
// Save the workbook
workbook.Save("BuiltinStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* enum [BuiltinStyleType](../../builtinstyletype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
