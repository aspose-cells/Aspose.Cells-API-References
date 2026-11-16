---
title: "UnionRange 类"
linktitle: "UnionRange"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "UnionRange 类。封装在 Go 中表示 unionrange 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/unionrange/
---

## UnionRange class

表示联合范围。

```go

type UnionRange struct  {
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
| [GetFirstRow](./getfirstrow/) | 获取范围第一行的索引。 |
| [GetFirstColumn](./getfirstcolumn/) | 获取范围第一列的索引。 |
| [GetRowCount](./getrowcount/) | 获取范围中行的数量。 |
| [GetColumnCount](./getcolumncount/) | 获取范围中行的数量。 |
| [Merge](./merge/) | 将一组单元格合并为单个单元格。 |
| [UnMerge](./unmerge/) | 取消合并此范围的已合并单元格。 |
| [PutValue](./putvalue/) | 将值放入范围中，如有必要，值将被转换为其他数据类型，且单元格的数字格式将被重置。 |
| [GetValue](./getvalue/) | 获取并设置范围的值。 |
| [SetValue](./setvalue/) | 获取并设置范围的值。 |
| [GetName](./getname/) | 获取或设置范围的名称。 |
| [SetName](./setname/) | 获取或设置范围的名称。 |
| [GetRefersTo](./getrefersto/) | 获取范围的引用。 |
| [GetHasRange](./gethasrange/) | 指示此项是否具有范围。 |
| [GetHyperlinks](./gethyperlinks/) | 获取范围内的所有超链接。 |
| [SetStyle](./setstyle/) | 设置范围的样式。 |
| [ApplyStyle](./applystyle/) | 对整个范围应用格式。 |
| [Copy](./copy/) | 使用粘贴特殊选项复制范围。 |
| [GetEnumerator](./getenumerator/) | 获取此 Range 中单元格的枚举器。 |
| [GetCellCount](./getcellcount/) | 获取范围内所有单元格的计数。 |
| [GetRangeCount](./getrangecount/) | 获取范围的数量。 |
| [GetRanges](./getranges/) | 获取所有联合范围。 |
| [SetOutlineBorders_CellBorderTypeArray_ColorArray](./setoutlineborders_cellbordertypearray_colorarray/) | 设置一组单元格的外框边界。 |
| [SetOutlineBorders_CellBorderType_Color](./setoutlineborders_cellbordertype_color/) | 为一组单元格设置相同边框样式和颜色的外框边界。 |
| [Intersect_String](./intersect_string/) | 与另一个范围相交。 |
| [Intersect_UnionRange](./intersect_unionrange/) | 与另一个范围相交。 |
| [Intersect_RangeArray](./intersect_rangearray/) | 与另一个范围相交。 |
| [Union_String](./union_string/) | 合并另一个范围。 |
| [Union_UnionRange](./union_unionrange/) | 合并另一个范围。 |
| [Union_RangeArray](./union_rangearray/) | 合并这些范围。 |
