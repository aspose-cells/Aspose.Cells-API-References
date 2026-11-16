---
title: "切片器类"
linktitle: "切片器"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "切片器类。封装在 Go 中表示切片器的对象。"
type: docs
weight: 200
url: /zh/go-cpp/slicer/
---

## Slicer class

切片器视图的摘要描述

```go

type Slicer struct  {
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
| [GetSortOrderType](./getsortordertype/) | 指示项目的排序类型。 |
| [SetSortOrderType](./setsortordertype/) | 指示项目的排序类型。 |
| [GetShowMissing](./getshowmissing/) | 指示是否显示已从数据源删除的项目。 |
| [SetShowMissing](./setshowmissing/) | 指示是否显示已从数据源删除的项目。 |
| [GetShowTypeOfItemsWithNoData](./getshowtypeofitemswithnodata/) | 指示是否显示已从数据源删除的项目。 |
| [SetShowTypeOfItemsWithNoData](./setshowtypeofitemswithnodata/) | 指示是否显示已从数据源删除的项目。 |
| [GetShowAllItems](./getshowallitems/) | 指示是否显示所有项目，即使没有数据或已被删除。默认值为 true； |
| [SetShowAllItems](./setshowallitems/) | 指示是否显示所有项目，即使没有数据或已被删除。默认值为 true； |
| [AddPivotConnection](./addpivotconnection/) | 添加数据透视表连接。 |
| [RemovePivotConnection](./removepivotconnection/) | 移除数据透视表连接。 |
| [GetLockedPosition](./getlockedposition/) | 指示指定的切片器是否可以通过用户界面移动或调整大小。 |
| [SetLockedPosition](./setlockedposition/) | 指示指定的切片器是否可以通过用户界面移动或调整大小。 |
| [Refresh](./refresh/) | 从关联的数据透视表刷新切片器的项目。 |
| [GetShape](./getshape/) | 返回与指定切片器关联的 Shape 对象。只读。 |
| [GetSlicerCache](./getslicercache/) | 返回与切片器关联的 SlicerCache 对象。只读。 |
| [GetWorksheet](./getworksheet/) | 返回包含此切片器的 Worksheet 对象。只读。 |
| [GetStyleType](./getstyletype/) | 指定内置切片器样式的类型。默认类型为 SlicerStyleLight1。 |
| [SetStyleType](./setstyletype/) | 指定内置切片器样式的类型。默认类型为 SlicerStyleLight1。 |
| [GetName](./getname/) | 返回或设置指定切片器的名称 |
| [SetName](./setname/) | 返回或设置指定切片器的名称 |
| [GetCaption](./getcaption/) | 返回或设置指定切片器的标题。 |
| [SetCaption](./setcaption/) | 返回或设置指定切片器的标题。 |
| [GetFirstItemIndex](./getfirstitemindex/) | 指定第一个切片器项目的零基索引。 |
| [SetFirstItemIndex](./setfirstitemindex/) | 指定第一个切片器项目的零基索引。 |
|[SelectItems](./selectitems/) |  | 
| [UnselectItems](./unselectitems/) | 移除选定的筛选标签。 |
| [ClearFilter](./clearfilter/) | 移除筛选 |
| [GetShowCaption](./getshowcaption/) | 指示切片器的标题是否可见。默认值为 true |
| [SetShowCaption](./setshowcaption/) | 指示切片器的标题是否可见。默认值为 true |
| [GetNumberOfColumns](./getnumberofcolumns/) | 返回或设置切片器中的列数。默认值为 1。 |
| [SetNumberOfColumns](./setnumberofcolumns/) | 返回或设置切片器中的列数。默认值为 1。 |
| [GetColumnWidthPixel](./getcolumnwidthpixel/) | 获取或设置切片器中每列的宽度，单位为像素。 |
| [SetColumnWidthPixel](./setcolumnwidthpixel/) | 获取或设置切片器中每列的宽度，单位为像素。 |
| [GetColumnWidth](./getcolumnwidth/) | 返回或设置切片器中每列的宽度，单位为点。 |
| [SetColumnWidth](./setcolumnwidth/) | 返回或设置切片器中每列的宽度，单位为点。 |
| [GetRowHeightPixel](./getrowheightpixel/) | 返回或设置指定切片器中每行的高度，单位为像素。 |
| [SetRowHeightPixel](./setrowheightpixel/) | 返回或设置指定切片器中每行的高度，单位为像素。 |
| [GetRowHeight](./getrowheight/) | 返回或设置指定切片器中每行的高度，单位为点。 |
| [SetRowHeight](./setrowheight/) | 返回或设置指定切片器中每行的高度，单位为点。 |
