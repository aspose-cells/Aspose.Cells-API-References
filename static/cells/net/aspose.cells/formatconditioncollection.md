##Class FormatConditionCollection
Aspose.Cells.FormatConditionCollection class. Represents conditional formatting. The FormatConditions can contain up to three conditional formats
## FormatConditionCollection class
Represents conditional formatting. The FormatConditions can contain up to three conditional formats.
```csharp
public class FormatConditionCollection
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells/formatconditioncollection/count/) { get; } | Gets the count of the conditions. |
| [Item](../../aspose.cells/formatconditioncollection/item/) { get; } | Gets the formatting condition by index. |
| [RangeCount](../../aspose.cells/formatconditioncollection/rangecount/) { get; } | Gets count of conditionally formatted ranges. |
## Methods
| Name | Description |
| --- | --- |
| [Add](../../aspose.cells/formatconditioncollection/add/)(CellArea, FormatConditionType, OperatorType, string, string) | Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting. |
| [AddArea](../../aspose.cells/formatconditioncollection/addarea/)(CellArea) | Adds a conditional formatted cell range. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition)(FormatConditionType) | Add a format condition. |
| [AddCondition](../../aspose.cells/formatconditioncollection/addcondition/#addcondition_1)(FormatConditionType, OperatorType, string, string) | Adds a formatting condition. |
| [GetCellArea](../../aspose.cells/formatconditioncollection/getcellarea/)(int) | Gets the conditional formatted cell range by index. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea_1)(int) | Removes conditional formatted cell range by index. |
| [RemoveArea](../../aspose.cells/formatconditioncollection/removearea/#removearea)(int, int, int, int) | Remove conditional formatting int the range. |
| [RemoveCondition](../../aspose.cells/formatconditioncollection/removecondition/)(int) | Removes the formatting condition by index. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FormatConditionCollectionDemo
{
public static void FormatConditionCollectionExample()
{
// Create a new Workbook
Workbook workbook = new Workbook();
// Get the first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Adds an empty conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
// Sets the conditional format range
CellArea ca = new CellArea { StartRow = 0, EndRow = 0, StartColumn = 0, EndColumn = 0 };
fcs.AddArea(ca);
ca = new CellArea { StartRow = 1, EndRow = 1, StartColumn = 1, EndColumn = 1 };
fcs.AddArea(ca);
// Adds conditions
int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
// Sets the background color
FormatCondition fc1 = fcs[conditionIndex1];
fc1.Style.BackgroundColor = System.Drawing.Color.Red;
// Saving the Excel file
workbook.Save("FormatConditionCollectionExample.xlsx");
workbook.Save("FormatConditionCollectionExample.pdf");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
