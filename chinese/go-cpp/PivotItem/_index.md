---
title: "PivotItem 类"
linktitle: "PivotItem"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotItem 类。封装在 Go 中表示 pivotitem 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotitem/
---

## PivotItem class

表示 PivotField 报表中的项目。

```go

type PivotItem struct  {
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
| [IsHidden](./ishidden/) | 获取和设置 pivot item 是否隐藏。 |
| [SetIsHidden](./setishidden/) | 获取和设置 pivot item 是否隐藏。 |
| [GetPosition](./getposition/) | 指定此项在该字段所有 PivotItems 中的索引。 |
| [SetPosition](./setposition/) | 指定此项在该字段所有 PivotItems 中的索引。 |
| [GetPositionInSameParentNode](./getpositioninsameparentnode/) | 指定同一父节点下的 PivotItems 中的位置索引。 |
| [SetPositionInSameParentNode](./setpositioninsameparentnode/) | 指定同一父节点下的 PivotItems 中的位置索引。 |
| [Move](./move/) | 将项向上或向下移动 |
| [IsDetailHidden](./isdetailhidden/) | 获取和设置此 pivot item 的详细信息是否隐藏。 |
| [SetIsDetailHidden](./setisdetailhidden/) | 获取和设置此 pivot item 的详细信息是否隐藏。 |
| [IsCalculatedItem](./iscalculateditem/) | 指示此 pivot item 是否为计算公式项。 |
| [GetFormula](./getformula/) | 获取此计算项的公式。仅在此项为计算项时有效。 |
| [IsMissing](./ismissing/) | 指示该项是否已从数据源中移除。 |
| [GetStringValue](./getstringvalue/) | 获取 pivot item 的字符串值。如果值为 null，则返回 ""。 |
| [GetDoubleValue](./getdoublevalue/) | 获取 pivot item 的双精度值。如果值为 null 或非数字，则返回 0。 |
| [GetDateTimeValue](./getdatetimevalue/) | 获取 pivot item 的日期时间值。如果值为 null，则返回 DateTime.MinValue。 |
| [GetValue](./getvalue/) | 获取 pivot item 的值 |
| [GetName](./getname/) | 获取 pivot item 的名称。 |
| [SetName](./setname/) | 获取 pivot item 的名称。 |
