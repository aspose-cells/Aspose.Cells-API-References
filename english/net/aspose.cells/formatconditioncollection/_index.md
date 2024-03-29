---
title: Class FormatConditionCollection
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.FormatConditionCollection class. Represents conditional formatting. The FormatConditions can contain up to three conditional formats
type: docs
url: /net/aspose.cells/formatconditioncollection/
---
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

[C#]

//Create a new Workbook.
Workbook workbook = new Workbook();

//Get the first worksheet.
Worksheet sheet = workbook.Worksheets[0];

//Adds an empty conditional formatting
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
//Sets the conditional format range.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.AddArea(ca);
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.AddArea(ca);
//Adds condition.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
//Adds condition.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
//Sets the background color.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
//Saving the Excel file
workbook.Save("output.xls");   

[Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
Dim sheet As Worksheet = workbook.Worksheets(0)
' Adds an empty conditional formatting
Dim index As Integer = sheet.ConditionalFormattings.Add()
Dim fcs As FormatConditionCollection = sheet.ConditionalFormattings(index)
'Sets the conditional format range.
Dim ca As CellArea = New CellArea()
ca.StartRow = 0
ca.EndRow = 0
ca.StartColumn = 0
ca.EndColumn = 0
fcs.AddArea(ca)
ca = New CellArea()
ca.StartRow = 1
ca.EndRow = 1
ca.StartColumn = 1
ca.EndColumn = 1
fcs.AddArea(ca)
'Adds condition.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100")
'Adds condition.
Dim conditionIndex2 As Integer = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100")
'Sets the background color.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
'Saving the Excel file
workbook.Save("output.xls")
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


