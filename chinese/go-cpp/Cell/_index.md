---
title: "Cell 类"
linktitle: "Cell"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Cell 类。封装在 Go 中表示 cell 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/cell/
---

## Cell class

封装表示单个工作簿单元格的对象。

```go

type Cell struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [Calculate](./calculate/) | 计算单元格的公式。 |
| [GetWorksheet](./getworksheet/) | 获取父工作表。 |
| [PutValue_Bool](./putvalue_bool/) | 向单元格写入布尔值。 |
| [PutValue_Int](./putvalue_int/) | 向单元格写入整数值。 |
| [PutValue_Double](./putvalue_double/) | 向单元格写入双精度值。 |
| [PutValue_String_Bool_Bool](./putvalue_string_bool_bool/) | 向单元格写入值，如有必要，值将被转换为其他数据类型，且单元格的数字格式将被重置。 |
| [PutValue_String_Bool](./putvalue_string_bool/) | 向单元格写入字符串值，并在适当时将该值转换为其他数据类型。 |
| [PutValue_String](./putvalue_string/) | 向单元格写入字符串值。 |
| [PutValue_Date](./putvalue_date/) | 向单元格写入 DateTime 值。 |
| [PutValue_Object](./putvalue_object/) | 向单元格写入对象值。 |
| [GetRow](./getrow/) | 获取单元格的行号（从零开始）。 |
| [GetColumn](./getcolumn/) | 获取单元格的列号（从零开始）。 |
| [IsFormula](./isformula/) | 表示指定单元格是否包含公式。 |
| [GetHasCustomFunction](./gethascustomfunction/) | 检查此单元格的公式中是否存在自定义函数（不受支持的函数）。 |
| [GetType](./gettype/) | 表示单元格的值类型。 |
| [GetName](./getname/) | 获取单元格的名称。 |
| [IsErrorValue](./iserrorvalue/) | 检查此单元格的值是否为错误。 |
| [IsNumericValue](./isnumericvalue/) | 指示此单元格的值是否为数值（int、double 和 datetime） |
| [GetStringValue_CellValueFormatStrategy](./getstringvalue_cellvalueformatstrategy/) | 通过特定的格式化策略获取字符串值。 |
| [GetStringValue](./getstringvalue/) | 获取单元格中的字符串值。如果此单元格的类型是字符串，则返回字符串本身。对于其他单元格类型，将返回格式化的字符串值（使用此单元格的指定样式进行格式化）。格式化后的单元格值与在 Excel 中将单元格复制为文本时（例如复制到文本编辑器或导出为 CSV）获得的值相同。 |
| [GetNumberCategoryType](./getnumbercategorytype/) | 表示此单元格数字格式的类别类型。 |
| [GetDisplayStringValue](./getdisplaystringvalue/) | 通过单元格的显示样式获取此单元格的格式化字符串值。 |
| [GetIntValue](./getintvalue/) | 获取单元格中的整数值。 |
| [GetDoubleValue](./getdoublevalue/) | 获取单元格中的双精度值。 |
| [GetFloatValue](./getfloatvalue/) | 获取单元格中的浮点值。 |
| [GetDateTimeValue](./getdatetimevalue/) | 获取单元格中的 DateTime 值。 |
| [GetBoolValue](./getboolvalue/) | 获取单元格中的布尔值。 |
| [GetWidthOfValue](./getwidthofvalue/) | 获取值的宽度，单位为像素。 |
| [GetHeightOfValue](./getheightofvalue/) | 获取值的高度，单位为像素。 |
| [GetDisplayStyle](./getdisplaystyle/) | 获取此单元格的显示样式。 |
| [GetDisplayStyle_Bool](./getdisplaystyle_bool/) | 获取此单元格的显示样式。 |
| [GetDisplayStyle_BorderType](./getdisplaystyle_bordertype/) | 获取此单元格的显示样式。 |
| [GetFormatConditions](./getformatconditions/) | 获取适用于此单元格的格式条件。 |
| [GetStyle](./getstyle/) | 获取单元格样式。 |
| [GetStyle_Bool](./getstyle_bool/) | 如果 checkBorders 为 true，则检查其他单元格的边框是否会影响此单元格的样式。 |
| [SetStyle_Style](./setstyle_style/) | 设置单元格样式。 |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | 将样式的已更改属性应用到单元格。 |
| [SetStyle_Style_StyleFlag](./setstyle_style_styleflag/) | 根据标志应用单元格样式。 |
| [GetHasCustomStyle](./gethascustomstyle/) | 指示此单元格是否具有自定义样式设置（不同于从相应行、列或工作簿继承的默认设置）。 |
| [GetSharedStyleIndex](./getsharedstyleindex/) | 获取单元格在样式池中的共享样式索引。 |
| [GetFormula](./getformula/) | 获取或设置单元格的公式。 |
| [SetFormula_String](./setformula_string/) | 获取或设置单元格的公式。 |
| [GetFormulaLocal](./getformulalocal/) | 获取单元格的本地化格式公式。 |
| [SetFormulaLocal](./setformulalocal/) | 获取单元格的本地化格式公式。 |
| [GetR1C1Formula](./getr1c1formula/) | 获取或设置单元格的 R1C1 公式。 |
| [SetR1C1Formula](./setr1c1formula/) | 获取或设置单元格的 R1C1 公式。 |
| [SetFormula_String_Object](./setformula_string_object/) | 设置公式及其值（计算结果）。 |
| [SetFormula_String_FormulaParseOptions](./setformula_string_formulaparseoptions/) | 设置公式及其值（计算结果）。 |
| [GetFormula_Bool_Bool](./getformula_bool_bool/) | 获取此单元格的公式。 |
| [SetFormula_String_FormulaParseOptions_Object](./setformula_string_formulaparseoptions_object/) | 设置公式及其值（计算结果）。 |
| [SetArrayFormula_String_Int_Int](./setarrayformula_string_int_int/) | 将数组公式（通过在 MS Excel 中按 CTRL+SHIFT+ENTER 输入的传统数组公式）设置到一组单元格。 |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions](./setarrayformula_string_int_int_formulaparseoptions/) | 将数组公式设置到一组单元格。 |
| [SetArrayFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setarrayformula_string_int_int_formulaparseoptions_object2array/) | 将数组公式设置到一组单元格。 |
| [SetSharedFormula_String_Int_Int](./setsharedformula_string_int_int/) | 将共享公式设置到一组单元格。 |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions](./setsharedformula_string_int_int_formulaparseoptions/) | 将共享公式设置到一组单元格。 |
| [SetSharedFormula_String_Int_Int_FormulaParseOptions_Object2Array](./setsharedformula_string_int_int_formulaparseoptions_object2array/) | 将共享公式设置到一组单元格。 |
| [GetContainsExternalLink](./getcontainsexternallink/) | 指示此单元格是否包含外部链接。仅在单元格为公式单元格时适用。 |
| [GetPrecedents](./getprecedents/) | 获取此单元格公式中出现的所有引用。 |
| [GetDependents](./getdependents/) | 获取所有公式直接引用此单元格的单元格。 |
| [GetPrecedentsInCalculation](./getprecedentsincalculation/) | 获取此单元格公式在计算时使用的所有前置单元格（对当前工作簿中单元格的引用）。 |
| [GetDependentsInCalculation](./getdependentsincalculation/) | 获取所有计算结果依赖于此单元格的单元格。 |
| [IsArrayHeader](./isarrayheader/) | 指示单元格的公式是数组公式且是该数组的首个单元格。 |
| [IsDynamicArrayFormula](./isdynamicarrayformula/) | 指示单元格的公式是动态数组公式（true）还是传统数组公式（false）。 |
| [GetArrayRange](./getarrayrange/) | 如果单元格的公式是数组公式，则获取其数组范围。 |
| [IsArrayFormula](./isarrayformula/) | 指示单元格公式是否为数组公式。 |
| [IsSharedFormula](./issharedformula/) | 指示单元格公式是否是共享公式的一部分。 |
| [IsTableFormula](./istableformula/) | 指示此单元格是否是表格公式的一部分。 |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Bool](./setdynamicarrayformula_string_formulaparseoptions_bool/) | 设置动态数组公式，并在可能的情况下使公式溢出到相邻单元格。 |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool/) | 设置动态数组公式，并在可能的情况下使公式溢出到相邻单元格。 |
| [SetDynamicArrayFormula_String_FormulaParseOptions_Object2Array_Bool_Bool_CalculationOptions](./setdynamicarrayformula_string_formulaparseoptions_object2array_bool_bool_calculationoptions/) | 设置动态数组公式，并在可能的情况下使公式溢出到相邻单元格。 |
| [SetTableFormula_Int_Int_String_String_Object2Array](./settableformula_int_int_string_string_object2array/) | 为给定范围创建双变量数据表，起始于此单元格。 |
| [SetTableFormula_Int_Int_String_Bool_Object2Array](./settableformula_int_int_string_bool_object2array/) | 为给定范围创建单变量数据表，起始于此单元格。 |
| [SetTableFormula_Int_Int_Int_Int_Int_Int_Object2Array](./settableformula_int_int_int_int_int_int_object2array/) | 为给定范围创建双变量数据表，起始于此单元格。 |
| [SetTableFormula_Int_Int_Int_Int_Bool_Object2Array](./settableformula_int_int_int_int_bool_object2array/) | 为给定范围创建单变量数据表，起始于此单元格。 |
| [RemoveArrayFormula](./removearrayformula/) | 移除数组公式。 |
| [Copy](./copy/) | 从源单元格复制数据。 |
| [GetValue](./getvalue/) | 获取/设置此单元格中包含的值。 |
| [SetValue](./setvalue/) | 获取/设置此单元格中包含的值。 |
| [IsStyleSet](./isstyleset/) | 指示单元格的样式是否已设置。如果返回 false，则表示此单元格使用默认单元格格式。 |
| [Characters](./characters/) | 返回一个 Characters 对象，表示单元格文本中一段字符范围。 |
| [Replace](./replace/) | 使用选项替换单元格的文本。 |
| [InsertText](./inserttext/) | 向单元格插入一些字符。如果单元格是富格式化的，此方法可以保留原始格式。 |
| [IsRichText](./isrichtext/) | 指示此单元格的字符串值是否为富格式化文本。 |
| [GetCharacters](./getcharacters/) | 返回所有 Characters 对象，表示单元格文本中一段字符范围。 |
| [GetCharacters_Bool](./getcharacters_bool/) | 返回所有 Characters 对象，表示单元格文本中一段字符范围。 |
| [SetCharacters](./setcharacters/) | 设置单元格的富文本格式。 |
| [IsMerged](./ismerged/) | 检查单元格是否是合并范围的一部分。 |
| [GetMergedRange](./getmergedrange/) | 返回一个 Range 对象，表示合并范围。 |
| [GetComment](./getcomment/) | 获取此单元格的批注。 |
| [GetHtmlString](./gethtmlstring/) | 获取和设置包含此单元格数据和部分格式的 HTML 字符串。 |
| [SetHtmlString](./sethtmlstring/) | 获取和设置包含此单元格数据和部分格式的 HTML 字符串。 |
| [GetHtmlString_Bool](./gethtmlstring_bool/) | 获取包含此单元格数据和部分格式的 HTML 字符串。 |
| [ToString](./tostring/) | 返回表示当前 Cell 对象的字符串。 |
| [ToJson](./tojson/) | 将 Cell 转换为 JSON 结构数据。 |
| [Equals_Object](./equals_object/) | 检查此对象是否与另一个对象引用同一单元格。 |
| [GetHashCode](./gethashcode/) | 作为特定类型的哈希函数。 |
| [Equals_Cell](./equals_cell/) | 检查此对象是否与另一个单元格对象引用同一单元格。 |
| [GetConditionalFormattingResult](./getconditionalformattingresult/) | 获取条件格式的结果。 |
| [GetValidation](./getvalidation/) | 获取应用于此单元格的验证。 |
| [GetValidationValue](./getvalidationvalue/) | 获取应用于此单元格的验证的值。 |
| [GetTable](./gettable/) | 获取包含此单元格的表。 |
| [IsCheckBoxStyle](./ischeckboxstyle/) | 指示是否将此单元格设置为复选框。 |
| [SetIsCheckBoxStyle](./setischeckboxstyle/) | 指示是否将此单元格设置为复选框。 |
| [GetRichValue](./getrichvalue/) | 获取单元格的富值。 |
| [GetEmbeddedImage](./getembeddedimage/) | 获取和设置单元格中的嵌入图像。 |
| [SetEmbeddedImage](./setembeddedimage/) | 获取和设置单元格中的嵌入图像。 |
| [GetPicture](./getpicture/) | 获取一个 Aspose.Cells.Drawing.Picture 实例，用于表示此单元格中的嵌入图像；如果此单元格没有嵌入图像，则返回 null。 |
|[Dispose](./dispose/) |  | 
