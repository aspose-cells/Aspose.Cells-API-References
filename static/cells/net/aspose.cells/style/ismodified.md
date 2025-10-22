##Style.IsModified
Style method. Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell
## Style.IsModified method
Checks whether the specified properties of the style have been modified. Used for style of ConditionalFormattings to check whether the specified properties of this style should be used when applying the ConditionalFormattings on a cell.
```csharp
public bool IsModified(StyleModifyFlag modifyFlag)
```
| Parameter | Type | Description |
| --- | --- | --- |
| modifyFlag | StyleModifyFlag | Style modified flags |
### Return Value
true if the specified properties have been modified
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StyleMethodIsModifiedWithStyleModifyFlagDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Get the style of cell A1
Style style = worksheet.Cells["A1"].GetStyle();
// Modify the pattern (background) of the style
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = System.Drawing.Color.Yellow;
// Check if the pattern was modified
bool isPatternModified = style.IsModified(StyleModifyFlag.Pattern);
// Output the result
Console.WriteLine("Is pattern modified: " + isPatternModified);
}
}
}
```
### See Also
* enum [StyleModifyFlag](../../stylemodifyflag/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
