---
title: GridCell
second_title: Aspose.Cells for .NET API 参考
description: 表示一个单元格对象
type: docs
weight: 370
url: /zh/net/aspose.cells.griddesktop.data/gridcell/
---
## GridCell class

表示一个单元格对象。

```csharp
public class GridCell
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BoolValue](../../aspose.cells.griddesktop.data/gridcell/boolvalue) { get; } | 获取单元格中包含的布尔值。 |
| [Column](../../aspose.cells.griddesktop.data/gridcell/column) { get; } | 获取单元格的列号（从零开始）。 |
| [DateValue](../../aspose.cells.griddesktop.data/gridcell/datevalue) { get; } | 获取单元格中包含的 DateTime 值。 |
| [DisplayStringValue](../../aspose.cells.griddesktop.data/gridcell/displaystringvalue) { get; } | 获取此单元格的格式化字符串值。 |
| [DoubleValue](../../aspose.cells.griddesktop.data/gridcell/doublevalue) { get; } | 获取单元格中包含的双精度值。 |
| [FloatValue](../../aspose.cells.griddesktop.data/gridcell/floatvalue) { get; } | 获取单元格中包含的浮点值。 |
| [Formula](../../aspose.cells.griddesktop.data/gridcell/formula) { get; set; } | 获取或设置公式Cell. |
| [HtmlString](../../aspose.cells.griddesktop.data/gridcell/htmlstring) { get; set; } | 获取和设置包含此单元格中的数据和一些格式的 html 字符串。 |
| [IntValue](../../aspose.cells.griddesktop.data/gridcell/intvalue) { get; } | 获取单元格中包含的整数值。 |
| [IsStyleSet](../../aspose.cells.griddesktop.data/gridcell/isstyleset) { get; } | 指示是否设置了单元格的样式。如果返回 false，则表示此单元格具有默认单元格格式。 |
| [Location](../../aspose.cells.griddesktop.data/gridcell/location) { get; } |  |
| [Name](../../aspose.cells.griddesktop.data/gridcell/name) { get; } | 获取单元格的名称。 例如：A1，F102。 |
| [Protected](../../aspose.cells.griddesktop.data/gridcell/protected) { get; set; } | 表示单元格是否受保护。 如果值为“true”，则用户无法通过用户界面修改单元格。 此属性与 Style.CellLocked 属性无关 不会保存到文件中网格数据导出。 默认值为“false”。 |
| [Row](../../aspose.cells.griddesktop.data/gridcell/row) { get; } | 获取单元格的行号（从零开始）。 |
| [StringValue](../../aspose.cells.griddesktop.data/gridcell/stringvalue) { get; } | 获取单元格中包含的字符串值。 |
| [Style](../../aspose.cells.griddesktop.data/gridcell/style) { get; set; } | 获取单元格样式的副本。设置单元格的样式。 |
| [Type](../../aspose.cells.griddesktop.data/gridcell/type) { get; } | 返回单元格值类型，含义见GridCellValueType.java |
| [Value](../../aspose.cells.griddesktop.data/gridcell/value) { get; set; } | 获取此单元格中包含的值。 |
| [Worksheet](../../aspose.cells.griddesktop.data/gridcell/worksheet) { get; } | 获取工作表对象。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [ContainsExternalLink](../../aspose.cells.griddesktop.data/gridcell/containsexternallink)() | 指示此单元格是否包含外部链接。 仅当单元格是公式单元格时适用。 |
| [Copy](../../aspose.cells.griddesktop.data/gridcell/copy)(GridCell) | 从源单元格复制数据。 |
| [CopyStyle](../../aspose.cells.griddesktop.data/gridcell/copystyle)(Style) | 复制样式并为单元格设置样式 |
| override [Equals](../../aspose.cells.griddesktop.data/gridcell/equals)(object) |  |
| [GetCellArea](../../aspose.cells.griddesktop.data/gridcell/getcellarea)() |  |
| [GetFont](../../aspose.cells.griddesktop.data/gridcell/getfont)() | 获取单元格字体。 更改字体时，应调用“SetFont”方法， 为单元格设置字体。 |
| [GetFontColor](../../aspose.cells.griddesktop.data/gridcell/getfontcolor)() | 获取单元格字体颜色。 更改颜色时，应调用“SetFontColor”方法， 设置单元格字体颜色。 |
| override [GetHashCode](../../aspose.cells.griddesktop.data/gridcell/gethashcode)() |  |
| [GetStyle](../../aspose.cells.griddesktop.data/gridcell/getstyle)() | 获取单元格样式。 更改样式时，应调用“SetStyle”方法， 为单元格设置样式。 |
| [GetValidation](../../aspose.cells.griddesktop.data/gridcell/getvalidation)() | 获取应用于此单元格的验证。如果未设置，则返回 null。 |
| [GetWidthOfValue](../../aspose.cells.griddesktop.data/gridcell/getwidthofvalue)() | 以像素为单位获取值的宽度。 |
| [GetWorksheet](../../aspose.cells.griddesktop.data/gridcell/getworksheet)() | 获取父工作表。 |
| [IsErrorValue](../../aspose.cells.griddesktop.data/gridcell/iserrorvalue)() | 检查公式是否可以正确评估结果。 |
| [IsFormula](../../aspose.cells.griddesktop.data/gridcell/isformula)() | 表示指定单元格是否包含公式。 |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue)(bool) | 将布尔值放入单元格中。 |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_3)(DateTime) | 将 DateTime 值放入单元格中。 |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_1)(double) | 将双精度值放入单元格中。 |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_2)(int) | 将一个 int 值放入单元格中。 |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_4)(object) | 将对象值放入单元格中。与 setValue(Object param_object) 相同 |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_5)(string) | 将字符串值放入单元格中。 |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_6)(string, bool) | 将字符串值放入单元格中，并在适当时将该值转换为其他数据类型。 |
| [PutValue](../../aspose.cells.griddesktop.data/gridcell/putvalue#putvalue_7)(string, bool, bool) | 将一个值放入单元格中，如果合适，该值将转换为其他数据类型，并且单元格的数字格式将被重置。 |
| [PutValueAndSetFormatByValue](../../aspose.cells.griddesktop.data/gridcell/putvalueandsetformatbyvalue)(string) | 使用字符串值设置单元格的值，并通过该值设置单元格格式。 |
| [SetCellValue](../../aspose.cells.griddesktop.data/gridcell/setcellvalue)(object) | 如果值为公式，此方法将单元格的值设置为公式类型， |
| [SetCustom](../../aspose.cells.griddesktop.data/gridcell/setcustom)(string) | 设置自定义格式，null 或空字符串表示没有自定义格式。 |
| [SetFont](../../aspose.cells.griddesktop.data/gridcell/setfont)(Font) | 为单元格设置字体。 为提高性能，实现“SetFont”方法， 不实现“字体”属性。 |
| [SetFontColor](../../aspose.cells.griddesktop.data/gridcell/setfontcolor)(Color) | 为单元格设置字体颜色。 为了提高性能，实现“SetFontColor”方法， 不实现“FontColor”属性。 |
| [SetFormula](../../aspose.cells.griddesktop.data/gridcell/setformula)(string, object) | 设置公式和公式的值。 |
| [SetNumberType](../../aspose.cells.griddesktop.data/gridcell/setnumbertype)(int) | 设置数字和日期的显示格式 |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcell/setstyle)(Style) | 为单元格设置样式。 为提高性能，实现“SetStyle”方法， 不实现“样式”属性。 |
| [ToString](../../aspose.cells.griddesktop.data/gridcell/tostring#tostring)() | 返回代表当前 Cell 对象的字符串。 |
| [operator ==](../../aspose.cells.griddesktop.data/gridcell/op_equality) |  |
| [operator !=](../../aspose.cells.griddesktop.data/gridcell/op_inequality) |  |

### 也可以看看

* 命名空间 [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* 部件 [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
