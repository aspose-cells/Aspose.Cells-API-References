---
title: "Range 类"
linktitle: "Range"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "Range 类。封装在 Go 中表示 range 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/range/
---

## Range class

封装表示电子表格中单元格范围的对象。

```go

type Range struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewRange_CellArea_Cells](./newrange_cellarea_cells/) | 类构造函数。 |
| [NewRange_Int_Int_Int_Int_Cells](./newrange_int_int_int_int_cells/) | 类构造函数。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [AutoFill_Range](./autofill_range/) | 自动填充目标范围。 |
| [AutoFill_Range_AutoFillType](./autofill_range_autofilltype/) | 自动填充目标范围。 |
| [GetCurrentRegion](./getcurrentregion/) | 返回一个表示当前区域的 Range 对象。当前区域是由任意组合的空行和空列界定的范围。 |
| [GetHyperlinks](./gethyperlinks/) | 获取范围内的所有超链接。 |
| [AddHyperlink](./addhyperlink/) | 向指定单元格或单元格范围添加超链接。 |
| [GetEnumerator](./getenumerator/) | 获取此 Range 中单元格的枚举器。 |
| [IsIntersect](./isintersect/) | 指示范围是否相交。 |
| [Intersect](./intersect/) | 返回一个表示两个范围矩形交集的 Range 对象。 |
| [UnionRanges](./unionranges/) | 返回两个范围的并集结果。 |
| [GetRowCount](./getrowcount/) | 获取范围中行的数量。 |
| [GetColumnCount](./getcolumncount/) | 获取范围中列的数量。 |
| [GetName](./getname/) | 获取或设置范围的名称。 |
| [SetName](./setname/) | 获取或设置范围的名称。 |
| [GetRefersTo](./getrefersto/) | 获取范围的引用。 |
| [GetAddress](./getaddress/) | 获取范围的地址。 |
| [IsBlank](./isblank/) | 指示范围是否包含值。 |
| [GetLeft](./getleft/) | 获取列 A 左边缘到范围左边缘的距离（单位：点）。 |
| [GetTop](./gettop/) | 获取行 1 顶部边缘到范围顶部边缘的距离（单位：点）。 |
| [GetWidth](./getwidth/) | 获取范围的宽度（单位：点）。 |
| [GetHeight](./getheight/) | 获取范围的宽度（单位：点）。 |
| [GetFirstRow](./getfirstrow/) | 获取范围第一行的索引。 |
| [GetFirstColumn](./getfirstcolumn/) | 获取范围第一列的索引。 |
| [Merge](./merge/) | 将一组单元格合并为单个单元格。 |
| [UnMerge](./unmerge/) | 取消合并此范围的已合并单元格。 |
| [PutValue](./putvalue/) | 将值放入范围中，如有必要，值将被转换为其他数据类型，且单元格的数字格式将被重置。 |
| [GetValue](./getvalue/) | 获取并设置范围的值。 |
| [SetValue](./setvalue/) | 获取并设置范围的值。 |
| [SetStyle_Style_Bool](./setstyle_style_bool/) | 应用单元格样式。 |
| [ApplyStyle](./applystyle/) | 对整个范围应用格式。 |
| [SetStyle_Style](./setstyle_style/) | 设置范围的样式。 |
| [SetOutlineBorders_CellBorderType_CellsColor](./setoutlineborders_cellbordertype_cellscolor/) | 为一组单元格设置相同边框样式和颜色的外框边界。 |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | 为一组单元格设置相同边框样式和颜色的外框边界。 |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | 设置一组单元格的外框边界。 |
| [SetOutlineBorder_BorderType_CellBorderType_CellsColor](./setoutlineborder_bordertype_cellbordertype_cellscolor/) | 设置一组单元格的外框边界。 |
| [SetOutlineBorder_BorderType_CellBorderType_Color](./setoutlineborder_bordertype_cellbordertype_color/) | 设置一组单元格的外框边界。 |
| [SetInsideBorders](./setinsideborders/) | 设置范围的内部边框。 |
| [GetColumnWidth](./getcolumnwidth/) | 设置或获取此范围的列宽。 |
| [SetColumnWidth](./setcolumnwidth/) | 设置或获取此范围的列宽。 |
| [GetRowHeight](./getrowheight/) | 设置或获取此范围内行的高度。 |
| [SetRowHeight](./setrowheight/) | 设置或获取此范围内行的高度。 |
| [MoveTo](./moveto/) | 将当前范围移动到目标范围。 |
| [CopyData](./copydata/) | 从源范围复制单元格数据（包括公式）。 |
| [CopyValue](./copyvalue/) | 从源范围复制单元格值。 |
| [CopyStyle](./copystyle/) | 从源范围复制样式设置。 |
| [Copy_Range_PasteOptions](./copy_range_pasteoptions/) | 使用粘贴特殊选项复制范围。 |
| [Transpose](./transpose/) | 转置（旋转）数据，将行转换为列或反之。 |
| [Copy_Range](./copy_range/) | 从源范围复制数据（包括公式）、格式、绘图对象等。 |
| [Get](./get/) | 获取此范围内的 Cell 对象。 |
| [GetCellOrNull](./getcellornull/) | 获取此范围内的 Cell 对象或 null。 |
| [GetOffset](./getoffset/) | 通过偏移获取 Range 范围。 |
| [GetEntireColumn](./getentirecolumn/) | 获取一个表示包含指定范围的整列（或多列）的 Range 对象。 |
| [GetEntireRow](./getentirerow/) | 获取一个表示包含指定范围的整行（或多行）的 Range 对象。 |
| [GetWorksheet](./getworksheet/) | 获取包含此范围的 Worksheet 对象。 |
| [ToString](./tostring/) | 返回表示当前 Range 对象的字符串。 |
| [ToImage](./toimage/) | 将范围转换为图像。 |
| [ToJson](./tojson/) | 将范围转换为 JSON 值。 |
| [ToHtml](./tohtml/) | 将范围转换为 HTML。 |
| [Clear](./clear/) | 清除此范围。 |
| [ClearContents](./clearcontents/) | 清除此范围的内容。 |
| [ClearFormats](./clearformats/) | 清除此范围的格式。 |
| [ClearComments](./clearcomments/) | 清除此范围的批注。 |
| [ClearHyperlinks](./clearhyperlinks/) | 仅移除超链接。 |
