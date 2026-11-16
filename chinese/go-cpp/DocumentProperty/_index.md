---
title: "DocumentProperty 类"
linktitle: "DocumentProperty"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "DocumentProperty 类。封装在 Go 中表示文档属性的对象。"
type: docs
weight: 200
url: /zh/go-cpp/documentproperty/
---

## DocumentProperty class

表示自定义或内置文档属性。

```go

type DocumentProperty struct  {
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
| [GetName](./getname/) | 返回属性的名称。 |
| [GetValue](./getvalue/) | 获取或设置属性的值。 |
| [SetValue](./setvalue/) | 获取或设置属性的值。 |
| [IsLinkedToContent](./islinkedtocontent/) | 指示此属性是否链接到内容 |
| [GetSource](./getsource/) | 链接的内容来源。 |
| [GetType](./gettype/) | 获取属性的数据类型。 |
| [IsGeneratedName](./isgeneratedname/) | 如果此属性在 OLE2 存储中没有名称，并且仅为公共 API 生成了唯一名称，则返回 true。 |
| [ToString](./tostring/) | 以字符串形式返回属性值。 |
| [ToInt](./toint/) | 以整数形式返回属性值。 |
| [ToDouble](./todouble/) | 以双精度浮点数形式返回属性值。 |
| [ToDateTime](./todatetime/) | 以本地时区的 DateTime 形式返回属性值。 |
| [ToBool](./tobool/) | 以布尔值形式返回属性值。 |
