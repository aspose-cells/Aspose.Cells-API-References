---
title: GridCell
second_title: Aspose.Cells for .NET API 参考
description: 表示一个单元格对象
type: docs
weight: 150
url: /zh/net/aspose.cells.gridweb.data/gridcell/
---
## GridCell class

表示一个单元格对象。

```csharp
public class GridCell
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BoolValue](../../aspose.cells.gridweb.data/gridcell/boolvalue) { get; } | 获取单元格中包含的布尔值。 |
| [Column](../../aspose.cells.gridweb.data/gridcell/column) { get; } | 获取单元格的列号（从零开始）。 |
| [DateValue](../../aspose.cells.gridweb.data/gridcell/datevalue) { get; } | 获取单元格中包含的 DateTime 值。 |
| [DisplayStringValue](../../aspose.cells.gridweb.data/gridcell/displaystringvalue) { get; } | 获取此单元格的格式化字符串值。 |
| [DoubleValue](../../aspose.cells.gridweb.data/gridcell/doublevalue) { get; } | 获取单元格中包含的双精度值。 |
| [FloatValue](../../aspose.cells.gridweb.data/gridcell/floatvalue) { get; } | 获取单元格中包含的浮点值。 |
| [Formula](../../aspose.cells.gridweb.data/gridcell/formula) { get; set; } | 获取或设置Cell的公式。 |
| [HtmlString](../../aspose.cells.gridweb.data/gridcell/htmlstring) { get; set; } | 获取和设置包含此单元格中的数据和一些格式的 html 字符串。 |
| [IntValue](../../aspose.cells.gridweb.data/gridcell/intvalue) { get; } | 获取单元格中包含的整数值。 |
| [IsStyleSet](../../aspose.cells.gridweb.data/gridcell/isstyleset) { get; } | 指示是否设置了单元格的样式。如果返回 false，则表示此单元格具有默认单元格格式。 |
| [Name](../../aspose.cells.gridweb.data/gridcell/name) { get; } | 获取单元格的名称。 例如:A1、F102。 |
| [Row](../../aspose.cells.gridweb.data/gridcell/row) { get; } | 获取单元格的行号（从零开始）。 |
| [StringValue](../../aspose.cells.gridweb.data/gridcell/stringvalue) { get; } | 获取单元格中包含的字符串值。 |
| [Style](../../aspose.cells.gridweb.data/gridcell/style) { get; set; } | 获取单元格样式的副本。设置单元格的样式。 |
| [Type](../../aspose.cells.gridweb.data/gridcell/type) { get; } | 返回单元格值类型，含义见GridCellValueType.java |
| [Value](../../aspose.cells.gridweb.data/gridcell/value) { get; set; } | 获取此单元格中包含的值。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.gridweb.data/gridcell/containsexternallink)() | 表示此单元格是否包含外部链接。 仅当单元格是公式单元格时适用。 |
| [Copy](../../aspose.cells.gridweb.data/gridcell/copy)(GridCell) | 从源单元格复制数据。 |
| [CopyStyle](../../aspose.cells.gridweb.data/gridcell/copystyle)(GridTableItemStyle) | 复制样式并设置单元格的样式 |
| [CreateComment](../../aspose.cells.gridweb.data/gridcell/createcomment)(string, string, bool) | 为单元格创建注释对象。 |
| [CreateValidation](../../aspose.cells.gridweb.data/gridcell/createvalidation)(GridValidationType, bool) | 为单元格创建验证对象。 |
| override [Equals](../../aspose.cells.gridweb.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.gridweb.data/gridcell/getcellarea)() |  |
| [GetComment](../../aspose.cells.gridweb.data/gridcell/getcomment)() | 获取此单元格上的评论对象 |
| override [GetHashCode](../../aspose.cells.gridweb.data/gridcell/gethashcode)() |  |
| [GetWidthOfValue](../../aspose.cells.gridweb.data/gridcell/getwidthofvalue)() | 获取值的宽度，以像素为单位。 |
| [IsErrorValue](../../aspose.cells.gridweb.data/gridcell/iserrorvalue)() | 检查公式是否可以正确评估结果。 |
| [IsFormula](../../aspose.cells.gridweb.data/gridcell/isformula)() | 表示指定单元格是否包含公式。 |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue)(bool) | 将布尔值放入单元格中。 |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_3)(DateTime) | 将 DateTime 值放入单元格中。 |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_1)(double) | 将双精度值放入单元格。 |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_2)(int) | 将一个 int 值放入单元格中。 |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_4)(object) | 将对象值放入单元格。与 setValue(Object param_object) |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_5)(string) | 将字符串值放入单元格中。 |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_6)(string, bool) | 将字符串值放入单元格并在适当时将该值转换为其他数据类型。 |
| [PutValue](../../aspose.cells.gridweb.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | 将一个值放入单元格中，如果合适，该值将转换为其他数据类型，并且单元格的数字格式将被重置。 |
| [PutValueAndSetFormatByValue](../../aspose.cells.gridweb.data/gridcell/putvalueandsetformatbyvalue)(string) | 使用字符串值设置单元格的值，并通过该值设置单元格格式。 |
| [RemoveComment](../../aspose.cells.gridweb.data/gridcell/removecomment)() | 删除单元格的注释对象。 |
| [RemoveValidation](../../aspose.cells.gridweb.data/gridcell/removevalidation)() | 移除单元格的验证对象。 |
| [SetBorder](../../aspose.cells.gridweb.data/gridcell/setborder)(WebBorderStyle) | 设置单元格的边框（上、下、左、右），所有边框都具有相同的边框样式。 |
| [SetCustom](../../aspose.cells.gridweb.data/gridcell/setcustom)(string) | 设置自定义格式，null或空字符串表示没有自定义格式。 |
| [SetFormula](../../aspose.cells.gridweb.data/gridcell/setformula)(string, object) | 设置公式和公式的值。 |
| [SetNumberType](../../aspose.cells.gridweb.data/gridcell/setnumbertype)(int) | 设置数字和日期的显示格式 |
| [ToString](../../aspose.cells.gridweb.data/gridcell/tostring#tostring)() | 返回代表当前 Cell 对象的字符串。 |
| [operator ==](../../aspose.cells.gridweb.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.gridweb.data/gridcell/op_inequality) |  |

### 也可以看看

* 命名空间 [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* 部件 [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
