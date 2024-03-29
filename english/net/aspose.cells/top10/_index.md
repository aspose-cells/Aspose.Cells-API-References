---
title: Class Top10
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Top10 class. Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket as specified
type: docs
url: /net/aspose.cells/top10/
---
## Top10 class

Describe the Top10 conditional formatting rule. This conditional formatting rule highlights cells whose values fall in the top N or bottom N bracket, as specified.

```csharp
public class Top10
```

## Constructors

| Name | Description |
| --- | --- |
| [Top10](top10/)() | The default constructor. |

## Properties

| Name | Description |
| --- | --- |
| [IsBottom](../../aspose.cells/top10/isbottom/) { get; set; } | Get or set whether a "top/bottom n" rule is a "bottom n" rule. Default value is false. |
| [IsPercent](../../aspose.cells/top10/ispercent/) { get; set; } | Get or set whether a "top/bottom n" rule is a "top/bottom n percent" rule. Default value is false. |
| [Rank](../../aspose.cells/top10/rank/) { get; set; } | Get or set the value of "n" in a "top/bottom n" conditional formatting rule. If IsPercent is true, the value must between 0 and 100. Otherwise it must between 0 and 1000. Default value is 10. |

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
CellArea ca = CellArea.CreateCellArea(0, 0, 10, 10);
fcs.AddArea(ca);
 
//Adds condition.
int conditionIndex = fcs.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);   
//Sets the background color.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
Top10 top10 = fc.Top10;
//Set the Top N 
top10.Rank = 5;  
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
Dim ca As CellArea = CellArea.CreateCellArea(0, 0, 10, 10)
fcs.AddArea(ca)
 
'Adds condition.
Dim conditionIndex As Integer = fcs.AddCondition(FormatConditionType.Top10, OperatorType.None, null, null);   
'Sets the background color.
Dim fc As FormatCondition = fcs(conditionIndex)
fc.Style.BackgroundColor = Color.Red
Dim top10 as Top10  = fc.Top10
'Set the Top N 
top10.Rank = 5
'Saving the Excel file
workbook.Save("output.xls")
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


