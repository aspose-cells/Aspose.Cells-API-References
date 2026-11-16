---
title: "PivotShowValuesSetting 类"
linktitle: "PivotShowValuesSetting"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotShowValuesSetting 类。封装表示 Go 中 pivotshowvaluessetting 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotshowvaluessetting/
---

## PivotShowValuesSetting class

表示在使用 ShowDataAs 计算时显示值的设置。

```go

type PivotShowValuesSetting struct  {
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
| [GetCalculationType](./getcalculationtype/) | 表示在数据透视报告中如何显示数据字段的值。 |
| [SetCalculationType](./setcalculationtype/) | 表示在数据透视报告中如何显示数据字段的值。 |
| [GetBaseFieldIndex](./getbasefieldindex/) | 表示在使用 ShowDataAs 计算时的基字段。 |
| [SetBaseFieldIndex](./setbasefieldindex/) | 表示在使用 ShowDataAs 计算时的基字段。 |
| [GetBaseItemPositionType](./getbaseitempositiontype/) | 表示在使用 ShowDataAs 计算时基字段中基枢轴项的类型。仅对数据字段有效。由于 PivotItemPosition.Custom 仅用于读取，如果需要设置 PivotItemPosition.Custom，请设置 PivotField.BaseItemIndex 属性。 |
| [SetBaseItemPositionType](./setbaseitempositiontype/) | 表示在使用 ShowDataAs 计算时基字段中基枢轴项的类型。仅对数据字段有效。由于 PivotItemPosition.Custom 仅用于读取，如果需要设置 PivotItemPosition.Custom，请设置 PivotField.BaseItemIndex 属性。 |
| [GetBaseItemIndex](./getbaseitemindex/) | 表示在使用 ShowDataAs 计算时基字段中枢轴项的自定义索引。仅对数据字段有效。 |
| [SetBaseItemIndex](./setbaseitemindex/) | 表示在使用 ShowDataAs 计算时基字段中枢轴项的自定义索引。仅对数据字段有效。 |
