---
title: Cell
second_title: Aspose.Cells for .NET API 参考
description: 封装表示单个工作簿单元格的对象
type: docs
weight: 230
url: /zh/net/aspose.cells/cell/
---
## Cell class

封装表示单个工作簿单元格的对象。

```csharp
public class Cell
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [BoolValue](../../aspose.cells/cell/boolvalue) { get; } | 获取单元格中包含的布尔值。 |
| [Column](../../aspose.cells/cell/column) { get; } | 获取单元格的列号（从零开始）。 |
| [Comment](../../aspose.cells/cell/comment) { get; } | 获取此单元格的注释。 |
| [ContainsExternalLink](../../aspose.cells/cell/containsexternallink) { get; } | 指示此单元格是否包含外部链接。 仅当单元格是公式单元格时适用。 |
| [DateTimeValue](../../aspose.cells/cell/datetimevalue) { get; } | 获取单元格中包含的 DateTime 值。 |
| [DisplayStringValue](../../aspose.cells/cell/displaystringvalue) { get; } | 通过单元格的显示样式获取该单元格的格式化字符串值。 |
| [DoubleValue](../../aspose.cells/cell/doublevalue) { get; } | 获取单元格中包含的双精度值。 |
| [FloatValue](../../aspose.cells/cell/floatvalue) { get; } | 获取单元格中包含的浮点值。 |
| [Formula](../../aspose.cells/cell/formula) { get; set; } | 获取或设置[`Cell`](../cell)的公式。 |
| [FormulaLocal](../../aspose.cells/cell/formulalocal) { get; set; } | 获取单元格的区域设置格式公式。 |
| [HtmlString](../../aspose.cells/cell/htmlstring) { get; set; } | 获取和设置包含此单元格中的数据和某些格式的 html 字符串。 |
| [IntValue](../../aspose.cells/cell/intvalue) { get; } | 获取单元格中包含的整数值。 |
| [IsArrayFormula](../../aspose.cells/cell/isarrayformula) { get; } | 表示单元格公式是否为数组公式。 |
| [IsArrayHeader](../../aspose.cells/cell/isarrayheader) { get; } | 表示单元格的公式是和数组公式 并且它是数组的第一个单元格。 |
| [IsErrorValue](../../aspose.cells/cell/iserrorvalue) { get; } | 检查此单元格的值是否错误。 |
| [IsFormula](../../aspose.cells/cell/isformula) { get; } | 表示指定单元格是否包含公式。 |
| [IsMerged](../../aspose.cells/cell/ismerged) { get; } | 检查单元格是否是合并范围的一部分。 |
| [IsNumericValue](../../aspose.cells/cell/isnumericvalue) { get; } | 指示此单元格的内部值是否为数字（int、double 和 datetime） |
| [IsSharedFormula](../../aspose.cells/cell/issharedformula) { get; } | 指示单元格公式是否是共享公式的一部分。 |
| [IsStyleSet](../../aspose.cells/cell/isstyleset) { get; } | 指示是否设置了单元格的样式。如果返回 false，则表示此单元格具有默认单元格格式。 |
| [IsTableFormula](../../aspose.cells/cell/istableformula) { get; } | 指示此单元格是否是表格公式的一部分。 |
| [Name](../../aspose.cells/cell/name) { get; } | 获取单元格的名称。 |
| [NumberCategoryType](../../aspose.cells/cell/numbercategorytype) { get; } | 表示此单元格数字格式的类别类型。 |
| [R1C1Formula](../../aspose.cells/cell/r1c1formula) { get; set; } | 获取或设置[`Cell`](../cell)的 R1C1 公式。 |
| [Row](../../aspose.cells/cell/row) { get; } | 获取单元格的行号（从零开始）。 |
| [SharedStyleIndex](../../aspose.cells/cell/sharedstyleindex) { get; } | 获取单元格在样式池中的共享样式索引。 |
| [StringValue](../../aspose.cells/cell/stringvalue) { get; } | 获取单元格中包含的字符串值。如果此单元格的类型是字符串，则返回字符串值本身。 对于其他单元格类型，将返回格式化的字符串值（按照该单元格的指定样式格式化）。 格式化的单元格值与将单元格复制为文本时从 excel 中获取的值相同（例如 将单元格复制到文本编辑器或导出到 csv）。 |
| [Type](../../aspose.cells/cell/type) { get; } | 表示单元格值类型。 |
| [Value](../../aspose.cells/cell/value) { get; set; } | 获取此单元格中包含的值。 |
| [Worksheet](../../aspose.cells/cell/worksheet) { get; } | 获取父工作表。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Calculate](../../aspose.cells/cell/calculate#calculate)(CalculationOptions) | 计算单元格的公式。 |
| [Characters](../../aspose.cells/cell/characters)(int, int) | 返回一个 Characters 对象，该对象表示单元格文本中的字符范围。 |
| [Copy](../../aspose.cells/cell/copy)(Cell) | 从源单元格复制数据。 |
| [Equals](../../aspose.cells/cell/equals#equals)(Cell) | 检查此对象是否与另一个单元格对象引用同一个单元格。 |
| override [Equals](../../aspose.cells/cell/equals#equals_1)(object) | 检查此对象是否与另一个引用相同的单元格。 |
| [GetArrayRange](../../aspose.cells/cell/getarrayrange)() | 如果单元格的公式是数组公式，则获取数组范围。 |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters)() | 返回所有 Characters 对象 表示单元格文本中的字符范围。 |
| [GetCharacters](../../aspose.cells/cell/getcharacters#getcharacters_1)(bool) | 返回所有 Characters 对象 表示单元格文本中的字符范围。 |
| [GetConditionalFormattingResult](../../aspose.cells/cell/getconditionalformattingresult)() | 获取条件格式化的结果。 |
| [GetDependents](../../aspose.cells/cell/getdependents)(bool) | 获取公式直接引用该单元格的所有单元格。 |
| [GetDependentsInCalculation](../../aspose.cells/cell/getdependentsincalculation)(bool) | 获取计算结果依赖于该单元格的所有单元格。 |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle)() | 获取单元格的显示样式。 如果此单元格还受其他设置影响，例如条件格式、列表对象等， 则显示样式可能与 cell.GetStyle() 不同。 |
| [GetDisplayStyle](../../aspose.cells/cell/getdisplaystyle#getdisplaystyle_1)(bool) | 获取单元格的显示样式。 如果单元格是条件格式，则显示样式与cell.GetStyle()不同。 |
| [GetFormatConditions](../../aspose.cells/cell/getformatconditions)() | 获取适用于此单元格的格式条件。 |
| [GetFormula](../../aspose.cells/cell/getformula)(bool, bool) | 获取此单元格的公式。 |
| override [GetHashCode](../../aspose.cells/cell/gethashcode)() | 用作特定类型的哈希函数。 |
| [GetHeightOfValue](../../aspose.cells/cell/getheightofvalue)() | 以像素为单位获取值的高度。 |
| [GetHtmlString](../../aspose.cells/cell/gethtmlstring)(bool) | 获取包含此单元格中的数据和某些格式的 html 字符串。 |
| [GetMergedRange](../../aspose.cells/cell/getmergedrange)() | 返回代表合并范围的[`Range`](../range)对象。 |
| [GetPrecedents](../../aspose.cells/cell/getprecedents)() | 获取出现在此单元格公式中的所有引用。 |
| [GetPrecedentsInCalculation](../../aspose.cells/cell/getprecedentsincalculation)() | 获取此单元格公式在计算时使用的所有先例（引用当前工作簿中的单元格）。 |
| [GetStringValue](../../aspose.cells/cell/getstringvalue)(CellValueFormatStrategy) | 通过特定的格式化策略获取字符串值。 |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle)() | 获取单元格样式。 |
| [GetStyle](../../aspose.cells/cell/getstyle#getstyle_1)(bool) | 如果 checkBorders 为真，则检查其他单元格的边框是否会影响该单元格的样式。 |
| [GetTable](../../aspose.cells/cell/gettable)() | 获取包含此单元格的表格。 |
| [GetValidation](../../aspose.cells/cell/getvalidation)() | 获取应用于此单元格的验证。 |
| [GetValidationValue](../../aspose.cells/cell/getvalidationvalue)() | 获取应用于此单元格的验证值。 |
| [GetWidthOfValue](../../aspose.cells/cell/getwidthofvalue)() | 以像素为单位获取值的宽度。 |
| [IsRichText](../../aspose.cells/cell/isrichtext)() | 指示单元格字符串值是否为富文本。 |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue)(bool) | 将布尔值放入单元格中。 |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_3)(DateTime) | 将 DateTime 值放入单元格中。 |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_1)(double) | 将双精度值放入单元格中。 |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_2)(int) | 将整数值放入单元格中。 |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_4)(object) | 将对象值放入单元格中。 |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_5)(string) | 将字符串值放入单元格中。 |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_6)(string, bool) | 将字符串值放入单元格并在适当时将该值转换为其他数据类型。 |
| [PutValue](../../aspose.cells/cell/putvalue#putvalue_7)(string, bool, bool) | 将一个值放入单元格中，如果合适，该值将转换为其他数据类型，并且单元格的数字格式将被重置。 |
| [RemoveArrayFormula](../../aspose.cells/cell/removearrayformula)(bool) | 删除数组公式。 |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula)(string, int, int) | 将数组公式（在 ms excel 中通过 CTRL+SHIFT+ENTER 输入的旧数组公式）设置为单元格区域。 |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_1)(string, int, int, FormulaParseOptions) | 将数组公式设置为单元格区域。 |
| [SetArrayFormula](../../aspose.cells/cell/setarrayformula#setarrayformula_2)(string, int, int, FormulaParseOptions, object[][]) | 将数组公式设置为单元格区域。 |
| [SetCharacters](../../aspose.cells/cell/setcharacters)(FontSetting[]) | 设置单元格的富文本格式。 |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula)(string, FormulaParseOptions, bool) | 设置动态数组公式并尽可能使公式溢出到相邻单元格中。 |
| [SetDynamicArrayFormula](../../aspose.cells/cell/setdynamicarrayformula#setdynamicarrayformula_1)(string, FormulaParseOptions, object[][], bool, bool) | 设置动态数组公式并尽可能使公式溢出到相邻单元格中。 |
| [SetFormula](../../aspose.cells/cell/setformula#setformula_2)(string, object) | 设置公式和公式的值。 |
| [SetFormula](../../aspose.cells/cell/setformula#setformula)(string, FormulaParseOptions, object) | 设置公式和公式的值。 |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula)(string, int, int) | 将公式设置为单元格区域。 |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_1)(string, int, int, FormulaParseOptions) | 将公式设置为单元格区域。 |
| [SetSharedFormula](../../aspose.cells/cell/setsharedformula#setsharedformula_2)(string, int, int, FormulaParseOptions, object[][]) | 将公式设置为单元格区域。 |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle)(Style) | 设置单元格样式。 |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_2)(Style, bool) | 应用单元格样式。 |
| [SetStyle](../../aspose.cells/cell/setstyle#setstyle_1)(Style, StyleFlag) | 应用单元格样式。 |
| override [ToString](../../aspose.cells/cell/tostring)() | 返回代表当前 Cell 对象的字符串。 |

### 例子

```csharp
[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//将一个字符串放入一个cell
Cell cell = cells[0, 0];
cell.PutValue("Hello");

string first = cell.StringValue;
	
 //将一个整数放入一个cell
cell = cells["B1"];
cell.PutValue(12);

int second = cell.IntValue;

 //把一个double放入一个cell
cell = cells[0, 2];
cell.PutValue(-1.234);

double third = cell.DoubleValue;

 //将公式放入cell
cell = cells["D1"];
cell.Formula = "=B1 + C1";

 //把一个组合公式：“sum(average(b1,c1), b1)”放到b2

cell = cells["b2"];
cell.Formula = "=sum(average(b1,c1), b1)";

//设置cell

Style style = cell.GetStyle();
//设置背景颜色
style.BackgroundColor = Color.Yellow;
 //设置cell

style.Font.Name = "Courier New";
style.VerticalAlignment = TextAlignmentType.Top;
cell.SetStyle(style);



[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = exce.Worksheets(0).Cells

//将一个字符串放入一个 cell
Dim cell as Cell = cells(0, 0)
cell.PutValue("Hello")

Dim first as String = cell.StringValue
	
 //将一个整数放入一个cell
cell = cells("B1")
cell.PutValue(12)

Dim second as Integer = cell.IntValue

 //把一个double放入一个cell
cell = cells(0, 2)
cell.PutValue(-1.234)

Dim third as Double = cell.DoubleValue

 //将公式放入cell
cell = cells("D1")
cell.Formula = "=B1 + C1"

 //把一个组合公式：“sum(average(b1,c1), b1)”放到b2

cell = cells("b2")
cell.Formula = "=sum(average(b1,c1), b1)"
	
//设置cell

Dim style as Style = cell.GetStyle()

//设置背景颜色
style.BackgroundColor = Color.Yellow
//设置cell

style.Font.Name = "Courier New"
style.VerticalAlignment = TextAlignmentType.Top
cell.SetStyle(style)
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
