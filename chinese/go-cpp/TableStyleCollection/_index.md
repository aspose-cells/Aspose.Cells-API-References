---
title: "TableStyleCollection 类"
linktitle: "TableStyleCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "TableStyleCollection 类。封装在 Go 中表示 tablestylecollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/tablestylecollection/
---

## TableStyleCollection class

表示所有自定义表样式。

```go

type TableStyleCollection struct  {
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
| [GetDefaultTableStyleName](./getdefaulttablestylename/) | 获取并设置表格的默认样式名称。 |
| [SetDefaultTableStyleName](./setdefaulttablestylename/) | 获取并设置表格的默认样式名称。 |
| [GetDefaultPivotStyleName](./getdefaultpivotstylename/) | 获取并设置数据透视表的默认样式名称。 |
| [SetDefaultPivotStyleName](./setdefaultpivotstylename/) | 获取并设置数据透视表的默认样式名称。 |
| [AddTableStyle](./addtablestyle/) | 添加自定义表格样式。 |
| [AddPivotTableStyle](./addpivottablestyle/) | 添加自定义数据透视表样式。 |
| [Get_Int](./get_int/) | 通过索引获取表格样式。 |
| [Get_String](./get_string/) | 通过名称获取表格样式。 |
| [GetBuiltinTableStyle](./getbuiltintablestyle/) | 获取内置表格样式 |
| [GetCount](./getcount/) | 获取实例中包含的元素数量。 |
