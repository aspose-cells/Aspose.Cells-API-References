---
title: FormatCondition
second_title: Aspose.Cells for .NET API 参考
description: 表示条件格式化条件
type: docs
weight: 3560
url: /zh/net/aspose.cells/formatcondition/
---
## FormatCondition class

表示条件格式化条件。

```csharp
public class FormatCondition
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AboveAverage](../../aspose.cells/formatcondition/aboveaverage) { get; } | 获取条件格式的“AboveAverage”实例。 默认实例的规则突出显示 高于范围内所有值的平均值的单元格。 仅对 type = AboveAverage 有效。 |
| [ColorScale](../../aspose.cells/formatcondition/colorscale) { get; } | 获取条件格式的“ColorScale”实例。 默认实例是“green-yellow-red” 3ColorScale 。 仅对 type = ColorScale 有效。 |
| [DataBar](../../aspose.cells/formatcondition/databar) { get; } | 获取条件格式的“DataBar”实例。 默认实例的颜色是蓝色。 仅对类型为 DataBar 有效。 |
| [Formula1](../../aspose.cells/formatcondition/formula1) { get; set; } | 获取和设置与条件格式相关的值或表达式。 |
| [Formula2](../../aspose.cells/formatcondition/formula2) { get; set; } | 获取和设置与条件格式相关的值或表达式。 |
| [IconSet](../../aspose.cells/formatcondition/iconset) { get; } | 获取条件格式的“IconSet”实例。 默认实例的 IconSetType 是 TrafficLights31。 仅对 type = IconSet 有效。 |
| [Operator](../../aspose.cells/formatcondition/operator) { get; set; } | 获取和设置条件格式运算符类型。 |
| [Priority](../../aspose.cells/formatcondition/priority) { get; set; } | 此条件格式规则的优先级。此值用于确定应评估和呈现哪种 格式。较低的数值比 较高的数值具有更高的优先级，其中“1”是最高优先级。 |
| [StopIfTrue](../../aspose.cells/formatcondition/stopiftrue) { get; set; } | 真，当此规则评估为真时，不能对此规则应用具有较低优先级的规则。 仅适用于 Excel 2007； |
| [Style](../../aspose.cells/formatcondition/style) { get; set; } | 获取或设置条件格式单元格区域的样式。 |
| [Text](../../aspose.cells/formatcondition/text) { get; set; } | “文本包含”条件格式规则中的文本值。 仅对 type = containsText、notContainsText、beginsWith 和 endsWith 有效。 默认值为空。 |
| [TimePeriod](../../aspose.cells/formatcondition/timeperiod) { get; set; } | “日期发生……”条件格式规则中的适用时间段。 仅对 type = timePeriod 有效。 默认值为 TimePeriodType.Today。 |
| [Top10](../../aspose.cells/formatcondition/top10) { get; } | 获取条件格式的“Top10”实例。 默认实例的规则突出显示 值位于前 10 个括号中的单元格。 仅对类型为 Top10 有效。 |
| [Type](../../aspose.cells/formatcondition/type) { get; set; } | 获取并设置是否为条件格式Type。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1)(bool, bool) | 获取与此格式条件关联的值或表达式。 |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_2)(int, int) | 获取单元格条件格式的公式。 |
| [GetFormula1](../../aspose.cells/formatcondition/getformula1#getformula1_1)(bool, bool, int, int) | 获取单元格条件格式的值或表达式。 |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2)(bool, bool) | 获取与此格式条件关联的值或表达式。 |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_2)(int, int) | 获取单元格条件格式的公式。 |
| [GetFormula2](../../aspose.cells/formatcondition/getformula2#getformula2_1)(bool, bool, int, int) | 获取单元格条件格式的值或表达式。 |
| [SetFormula1](../../aspose.cells/formatcondition/setformula1)(string, bool, bool) | 设置与此格式条件关联的值或表达式。 |
| [SetFormula2](../../aspose.cells/formatcondition/setformula2)(string, bool, bool) | 设置与此格式条件关联的值或表达式。 |
| [SetFormulas](../../aspose.cells/formatcondition/setformulas)(string, string, bool, bool) | 设置与此格式条件关联的值或表达式。 |

### 例子

```csharp

[C#]
 //实例化一个工作簿对象
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
 
 //添加一个空的条件格式
int index = sheet.ConditionalFormattings.Add();
FormatConditionCollection fcs = sheet.ConditionalFormattings[index];
 
 //设置条件格式范围.
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
 
 //添加条件.
int conditionIndex = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
 
 //添加条件.
int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
 
 //设置背景颜色.
FormatCondition fc = fcs[conditionIndex];
fc.Style.BackgroundColor = Color.Red;
 
 //保存Excel文件
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

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
