---
title: FormatCondition
second_title: Aspose.Cells for .NET API Reference
description: Represents conditional formatting condition.
type: docs
weight: 3600
url: /net/aspose.cells/formatcondition/
---
## FormatCondition class

Represents conditional formatting condition.

```csharp
public class FormatCondition
```

## Properties

| Name | Description |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage) { get; } | Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage. |
| [ColorScale](../../aspose.cells/formatcondition/colorscale) { get; } | Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale. |
| [DataBar](../../aspose.cells/formatcondition/databar) { get; } | Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar. |
| [Formula1](../../aspose.cells/formatcondition/formula1) { get; set; } | Gets and sets the value or expression associated with conditional formatting. |
| [Formula2](../../aspose.cells/formatcondition/formula2) { get; set; } | Gets and sets the value or expression associated with conditional formatting. |
| [IconSet](../../aspose.cells/formatcondition/iconset) { get; } | Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet. |
| [Operator](../../aspose.cells/formatcondition/operator) { get; set; } | Gets and sets the conditional format operator type. |
| [Priority](../../aspose.cells/formatcondition/priority) { get; set; } | The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority. |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue) { get; set; } | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007; |
| [Style](../../aspose.cells/formatcondition/style) { get; set; } | Gets or setts style of conditional formatted cell ranges. |
| [Text](../../aspose.cells/formatcondition/text) { get; set; } | The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null. |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod) { get; set; } | The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today. |
| [Top10](../../aspose.cells/formatcondition/top10) { get; } | Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10. |
| [Type](../../aspose.cells/formatcondition/type) { get; set; } | Gets and sets whether the conditional format Type. |

## Methods

| Name | Description |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1)(bool, bool) | Gets the value or expression associated with this format condition. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_2)(int, int) | Gets the formula of the conditional formatting of the cell. |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_1)(bool, bool, int, int) | Gets the value or expression of the conditional formatting of the cell. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2)(bool, bool) | Gets the value or expression associated with this format condition. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_2)(int, int) | Gets the formula of the conditional formatting of the cell. |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_1)(bool, bool, int, int) | Gets the value or expression of the conditional formatting of the cell. |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1)(string, bool, bool) | Sets the value or expression associated with this format condition. |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2)(string, bool, bool) | Sets the value or expression associated with this format condition. |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas)(string, string, bool, bool) | Sets the value or expression associated with this format condition. |

### Examples

```csharp

[C#]
//Instantiating a Workbook object
Workbook workbook = new Workbook();
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

[VB.NET]

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

* namespace [Aspose.Cells](../../aspose.cells)
* assembly [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
